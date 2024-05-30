# Testing Strategy

Frame it more in terms of a testing strategy. And pick and chose what's most appropriate for the project based on constraints. Eg some tests are more time consuming then others (eg End to End) and others are more insightful to quickly identify a bug 🐛 (eg Integration tests)

Testing strategy that strikes the Right balance between adding confidence in the code base as well as ability to make changes without introducing bugs. Especially within a team.

Eg Snapshot test/screenshot testing can be potentially a premature optimization - definitely valuable for stable projects, but could indure progress on WIP MVP.

Type of tests at a high level

1. **Linting**, also kind of test to enforce best practices during development, at commit etc.. (ESLint)
2. **Typechecking**, eg PropTypes for React
3. **Unit test** - a single function or service (Jest)
4. **Component test** - a single component - functionality (jest/Enzyme)
5. **Snapshot Test** - a single component - visual regression testing, eg changes against previous versions (Jest, [percy.io](https://percy.io/), [backstopJS](https://garris.github.io/BackstopJS/))
6. **End to End Test** - Interaction between multiple components, usually from point of view of a user (Cypress)
7. **Performance test** - How the app performs in difference environment
8. **Coverage tests** - How much of your application of the app is covered by tests
9. **Browser Testing** -  Test how the app/page renders across browsers, devices and operating systems, manual or automated. Can return screenshots.(Browser Stack)
10. **Testing calls to API end points -** Test modules and/or components that perform HTTP requests in isolation, by mocking the server end points to validate the request ****- (Nock)

Also

- **QA** - Manual or automated, same dev team or dedicated team.
- **BDD** Tests - Behaviour driven development (cucumber)
- Tests can also be connected to deployment, eg to be run automatically in the background with PR reviews etc..

For more see 

[Testing Strategy - Draft](https://pietropassarelli.net/testing-strategy.html)

[Testing Overview - React](https://reactjs.org/docs/testing.html)

[Testing Recipes - React](https://reactjs.org/docs/testing-recipes.html)

[Testing Environments - React](https://reactjs.org/docs/testing-environments.html)