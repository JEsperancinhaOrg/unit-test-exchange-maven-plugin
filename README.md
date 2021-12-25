# unit-test-exchange-maven-plugin

This plugin works as a tool to convert unit tests from one standard to another. The goal is to support many times

## Options

| Option |Function| Source Code |Target Code| Status        |
|--------|---|-------------|---|---------------|
| 1      | Converts from JUnit, Mockito, Hamcrest/AssertJ to MockK, JUpiter and Kotest assertions| Kotlin      |Kotlin| Supported     |
| 2      | Converts from JUnit, Mockito, Hamcrest/AssertJ to MockK, JUpiter and Kotest assertions| Java        |Kotlin| InDevelopment |

## Before running this plugin

Make sure you have your code formatted according initial expectations as much as possible. The rules are:

1. Annotated methods in separate lines
2. Annotated test methods should have no space between parenthesis if they receive value directly as the following example:

```kotlin
@Test(expected = IOException::class)
fun testThisStuff() {
}
```

3. Make sure the source code and target code match the choice you make
4. Clean imports and make sure you removed all code not being used.
5. There are no 100% guarantees that the resulting code will compile and run immediately after you run this. Manual intervention afterward may be necessary.
