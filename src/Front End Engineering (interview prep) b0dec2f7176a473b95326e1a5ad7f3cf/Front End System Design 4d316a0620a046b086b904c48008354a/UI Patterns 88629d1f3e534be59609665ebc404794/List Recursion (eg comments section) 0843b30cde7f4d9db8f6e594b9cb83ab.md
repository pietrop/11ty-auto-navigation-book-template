# List Recursion (eg comments section)

```jsx
import React from "react"

const commentData = {
  title: "Fake article title.",
  author: "grzm",
  comments: [
    {
      id: 1,
      text: "Example comment here.",
      author: "user2",
      children: [
        {
          id: 2,
          text: "Another example comment text.",
          author: "user3",
          children: [
            {
              id: 3,
              text: "Another example comment text.",
              author: "user4",
              children: []
            }
          ]
        }
      ]
    },
    {
      id: 4,
      text: "Example comment here 2.",
      author: "user5",
      children: []
    }
  ]
}

function Comment({ comment }) {
  const nestedComments = (comment.children || []).map(comment => {
    return <Comment key={comment.id} comment={comment} type="child" />
  })

  return (
    <div style={{"marginLeft": "25px", "marginTop": "10px"}}>
      <div>{comment.text}</div>
      {nestedComments}
    </div>
  )
}

function App() {
  return (
    <div>
      {
        commentData.comments.map((comment) => {
          return (
            <Comment key={comment.id} comment={comment} />
          )
        })
      }
    </div>
  )
}

export default App
```

[Recursion in React: Render Comments with Nested Children](https://coderrocketfuel.com/article/recursion-in-react-render-comments-with-nested-children)

[List Recursion (eg comments section)]()

[Build nested commenting system using Laravel and VueJs - Part 1](https://scotch.io/@jagadeshanh/build-nested-commenting-system-using-laravel-and-vuejs-part-1)

SQL pattern

[Managing Hierarchical Data in MySQL - Mike Hillyer's Personal Webspace](http://mikehillyer.com/articles/managing-hierarchical-data-in-mysql/)