# Espresso 

Use Espresso to write concise, beautiful, and reliable Android UI tests.

The following code snippet shows an example of an Espresso test:

@Test
public void greeterSaysHello() {
    onView(withId(R.id.name_field)).perform(typeText("Steve"));
    onView(withId(R.id.greet_button)).perform(click());
    onView(withText("Hello Steve!")).check(matches(isDisplayed()));
}

![image](../img/espresso.png)

## Target audience

Espresso is targeted at developers, who believe that automated testing is an integral part of the development lifecycle. While it can be used for black-box testing, Espresso’s full power is unlocked by those who are familiar with the codebase under test.

## Packages

- espresso-core - Contains core and basic View matchers, actions, and assertions. See Basics and Recipes.
- espresso-web - Contains resources for WebView support.
- espresso-idling-resource - Espresso's mechanism for synchronization with background jobs.
- espresso-contrib - External contributions that contain DatePicker, RecyclerView and Drawer actions, accessibility checks, and CountingIdlingResource.
- espresso-intents - Extension to validate and stub intents for hermetic testing.
- espresso-remote - Location of Espresso's multi-process functionality.

## Create UI tests with Espresso Test Recorder 

The Espresso Test Recorder tool lets you create UI tests for your app without writing any test code. By recording a test scenario, you can record your interactions with a device and add assertions to verify UI elements in particular snapshots of your app. Espresso Test Recorder then takes the saved recording and automatically generates a corresponding UI test that you can run to test your app.

## Record an Espresso test

### Record UI interactions

To start recording a test with Espresso Test Recorder, proceed as follows:

1. Click Run > Record Espresso Test.
2. In the Select Deployment Target window, choose the device on which you want to record the test. If necessary, create a new Android Virtual Device. Click OK.
3. Espresso Test Recorder triggers a build of your project, and the app must install and launch before Espresso Test Recorder allows you to interact with it. The Record Your Test window appears after the app launches, and since you have not interacted with the device yet, the main panel reads "No events recorded yet." Interact with your device to start logging events such as "tap" and "type" actions.

### Add assertions to verify UI elements

Assertions verify the existence or contents of a View element through three main types:

- text is: Checks the text content of the selected View element
- exists: Checks that the View element is present in the current View hierarchy visible on the screen
- does not exist: Checks that the View element is not present in the current View hierarchy

# To go deep in this section got to this link and follow the steps [Espresso test recorder](https://developer.android.com/studio/test/espresso-test-recorder)