# Testing

INTRO Text to (frontend) testing. This is an extension of the general Testing Standard.

- integration
- unit
- e2e
- snapshot

## Tests in Amsterdam frontend projects

- unit
  elke vorm logica moet getest worden
- integration
  wegmocken van externen afhankelijkheden.
  integratie test light
  maakt gebruik van JSDom kan een nadeel zijn.

## Testing strategy:

- Don't test [implementation detail](https://kentcdodds.com/blog/testing-implementation-details)
- what to test <https://kentcdodds.com/blog/write-tests>
- TODO: Best practices:
  - <https://www.benmvp.com/blog/react-testing-library-best-practices/>
  - <https://github.com/patternfly/patternfly-react/wiki/React-Testing-Library-Basics,-Best-Practices,-and-Guidelines>
- Mocking
  - organise your mocking `__mocks__`
  - fixtures `__stubs__`
- Project documentation for testing

## Test coverage

- line coverage
- branch coverage

## Tests part of deployment pipeline

## Best practices

- test niet 3rd party libraries
- gebruik testid(s)
- debuggen??

## debuggen??

## Tooling

- https://miragejs.com/
- editor extensions

## References

- <https://circleci.com/blog/unit-testing-vs-integration-testing/>
- [Snapshot testing](https://circleci.com/blog/snapshot-testing-with-jest/)
- <https://testing-library.com/docs/guiding-principles/>

## Advanced testing?

#### Notes from meeting with Rene:

- Testing gives more confidence in releasing software
- Mostly integration and unit tests
- Standarize mocking
- Don't test everything.
- Test mindset
  - key takeaways??
