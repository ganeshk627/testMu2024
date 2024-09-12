# Choosing the Right Framework: Exploring the Selenium Ecosystem for Testing

## Speaker: Diego Molina, Selenium Lead - OSPO Lead, Sauce Labs, Valencia

# Should You Choose Selenium?

### Yes
- 🟡 Cross-browser and cross-platform support
- 🟡 Based on a W3C standard
- 🟡 Local and remote execution
- 🟡 By the community, for the community

### No
- 🟡 Automatic waiting
- 🟡 Reporting
- 🟡 Assertions
- 🟡 Boilerplate code

# Selenium WebDriver
```mermaid
graph LR
    A(Web - 1993) --> B(Se WebDriver - 2004)
    B --> C(WebDriver - 2005)
    C --> D(Merged with Selenium WebDriver - 2009)
    D --> E(Selenium WebDriver - 2011-2014)
    E --> F(Became WebDriver Classic - 2017)
    F --> G(W3C WebDriver - 2018)
```

# WebDriver Ecosystem
## Tools and Libraries:
- **Nightwatch js**:
- **Appium/appium**: Cross-platform automation framework for all your apps built on iOS or Android.  
  ![Appium Logo](path_to_appium_image)
- **robotframework/SeleniumLibrary**: Web testing library for Robot Framework.  
  ![RobotFramework Logo](path_to_robotframework_image)
- **Selenium Basic**:
- **SerenityJS**: Helps you write cleaner, more maintainable acceptance tests.  
  ![SerenityJS Logo](path_to_serenityjs_image)
- **Laravel Dusk**: Provides an expressive, easy-to-use browser automation and testing API.  
  ![Laravel Dusk Logo](path_to_laravel_dusk_image)
- **Panther**: A standalone browser testing library for PHP.
  ![Panther Logo](path_to_panther_image)
- **watir/watir**: Web application testing in Ruby.
  ![Watir Logo](path_to_watir_image)
- **selenide/selenide**: Concise UI tests for Java.
  ![Selenide Logo](path_to_selenide_image)
- **atata-framework/atata**: C#/.NET test automation framework.
  ![Atata Logo](path_to_atata_image)
- **iamalittletester/waiter2**: Wait for elements to load in Selenium tests.
  ![Waiter2 Logo](path_to_waiter2_image)
- **titusfortner/selenium-logger**: Selenium logging in the browser.
  ![Selenium Logger Logo](path_to_selenium_logger_image)


## Implementations:
- **Selenium**: A browser automation framework and ecosystem.  
  ![Selenium Logo](path_to_selenium_image)
- **webdriverio/webdriverio**: Next-gen browser and mobile automation test framework for Node.js.  
  ![WebdriverIO Logo](path_to_webdriverio_image)
- **php-webdriver/php-webdriver**: PHP client for Selenium WebDriver project.  
  ![PHP WebDriver Logo](path_to_php_webdriver_image)

# JavaScript Rises
```mermaid
timeline
    title JavaScript Rises
    2009 : Node.js
    2011 : WebdriverIO ![WebdriverIO](link_to_image)
    2012 : Appium ![Appium](link_to_image)
    2013 : Protractor (Deprecated) ![Protractor](link_to_image)
    2014 : Nightwatch.js ![Nightwatch](link_to_image)
    2016 : TestCafe ![TestCafe](link_to_image)
    2017 : Cypress ![Cypress](link_to_image)
    2018 : Puppeteer ![Puppeteer](link_to_image)
    2020 : Playwright ![Playwright](link_to_image)
```

# Automation Approaches
```mermaid
graph TD
    A[Automation Approaches] 
    A --> HL[High Level]
    A --> LL[Low Level]

    HL --> B[Web APIs & Node.js]

    LL --> C[WebDriver 'Classic Protocol']
    LL --> D[Chrome DevTools Protocol -CDP]

    B --> E[Cypress]
    B --> F[TestCafe]

    C --> G[Selenium]
    C --> H[WebdriverIO]
    C --> I[Appium]
    C --> J[Nightwatch]

    D --> K[Puppeteer]
    D --> L[Playwright -modified]

    style A fill:#10F310,stroke:#444,stroke-width:5px;
    style HL fill:#F1F3F4,stroke:#333,stroke-width:2px;
    style LL fill:#F1F3F4,stroke:#333,stroke-width:2px;
    style B fill:#F1F3F4,stroke:#333,stroke-width:2px;
    style C fill:#F1F3F4,stroke:#333,stroke-width:2px;
    style D fill:#F1F3F4,stroke:#333,stroke-width:2px;
```


# High-level - Cypress

### Node.js Process:
- Starts with Proxy
- Handles HTTP Requests and Responses

### Browser:
- Cypress tests with Application, manipulating DOM, Window, etc.

---

# High-level - TestCafe

### Browser Interaction:
- Opens page, sends and receives requests through the server

### TestCafe:
- Emulates requests and responses
- Injects autonomous scripts



# WebDriver 'Classic' Vs 'CDP'
```mermaid
graph LR
    A[Automation Tools] --> B[Browser Drivers]
    B --> C[Browsers - W3C Standard: Chrome, Firefox, etc.]

    D[Automation Tools - CDP] --> E[WebSocket]
    E --> F[Chromium-based Browsers]
```

# Low-Level Controls
1. Capturing console messages
2. Intercepting network requests
3. Simulating device mode
4. Simulating geolocation
5. And more!

# WebDriver BiDi Ecosystem
## Tools and Libraries:
- **Nightwatch js**:
- **Appium/appium**: Cross-platform automation framework for all your apps built on iOS or Android.  
  ![Appium Logo](path_to_appium_image)
- **robotframework/SeleniumLibrary**: Web testing library for Robot Framework.  
  ![RobotFramework Logo](path_to_robotframework_image)
- **Selenium Basic**:
- **SerenityJS**: Helps you write cleaner, more maintainable acceptance tests.  
  ![SerenityJS Logo](path_to_serenityjs_image)
- **Laravel Dusk**: Provides an expressive, easy-to-use browser automation and testing API.  
  ![Laravel Dusk Logo](path_to_laravel_dusk_image)
- **Panther**: A standalone browser testing library for PHP.
  ![Panther Logo](path_to_panther_image)
- **watir/watir**: Web application testing in Ruby.
  ![Watir Logo](path_to_watir_image)
- **selenide/selenide**: Concise UI tests for Java.
  ![Selenide Logo](path_to_selenide_image)
- **atata-framework/atata**: C#/.NET test automation framework.
  ![Atata Logo](path_to_atata_image)
- **iamalittletester/waiter2**: Wait for elements to load in Selenium tests.
  ![Waiter2 Logo](path_to_waiter2_image)
- **titusfortner/selenium-logger**: Selenium logging in the browser.
  ![Selenium Logger Logo](path_to_selenium_logger_image)


## Implementations:
- **Selenium**: A browser automation framework and ecosystem.  
  ![Selenium Logo](path_to_selenium_image)
- **webdriverio/webdriverio**: Next-gen browser and mobile automation test framework for Node.js.  
  ![WebdriverIO Logo](path_to_webdriverio_image)
- **php-webdriver/php-webdriver**: PHP client for Selenium WebDriver project.  
  ![PHP WebDriver Logo](path_to_php_webdriver_image)
- **puppeteer/puppeteer**:


# Features to Look For

- **Assertions on actions**
- **Initialization and cleanup**
- **Data modeling/mocking**
- **Configuration**
- **Wrappers and helpers**
- **API usage**
- **Future-ready features**
- **Local and cloud setups**
- **Speed and debugging features**
- **Cross-browser, simulators, emulators**
- **Built-in reporting**

---

# What Else Should I Consider?

- **Programming language**
- **Repository activity** (issues, stars, pull requests)
- **Support channels**
- **Documentation**
- **Proof of concept**
- **Governance**



# Java - Selenide

## Key Features:
- **Concise fluent API for tests**
- **Stable tests**
- **Powerful selectors**
- **Simple configuration**

## Sample Login Test:

```java
@Test
public void userCanLogin() {
    open("https://the-internet.herokuapp.com/login");
    $("#username").setValue("tomsmith");
    $("#password").setValue("SuperSecretPassword!").pressEnter();
    $("#flash").shouldHave(text("You logged into a secure area!"));
}
```

## Error Messages:
```bash
Element should be hidden {#gameWin}
Element: '<img class="gameOver" id="gameWin" src="img/thumbs-up.jpeg"></img>'
Screenshot: file:/.../hangman/build/reports/tests/1510751914648.0.png
Page source: file:/.../hangman/build/reports/tests/1510751914648.0.html
Timeout: 4 s.
```

# Tools Overview

### Watir
- **Watir**: An open-source Ruby library for automating tests. It provides a simple and efficient way to interact with web browsers through scripts.
  - **Features**:
    - Concise fluent API for tests
    - Stable tests with powerful selectors
    - Simple configuration
    - Supports extensive testing capabilities

### WebdriverIO
- **WebdriverIO**: A next-generation automation test framework for Node.js. It facilitates browser and mobile automation, integrating seamlessly into modern development workflows.
  - **Features**:
    - Supports synchronous and asynchronous execution
    - Extensible and customizable, fitting various testing needs
    - Rich ecosystem with numerous plugins

### Playwright
- **Playwright**: A JavaScript framework designed for reliable end-to-end testing of modern web applications. It provides robust testing features that support all major browsers.
  - **Features**:
    - Cross-browser and cross-platform testing
    - Handles both headless and non-headless modes
    - Powerful automation capabilities with a single API

### Atata
- **Atata**: A .NET/C# full-featured framework for automated web testing, designed to provide a comprehensive solution for enterprise environments.
  - **Features**:
    - Based on Selenium WebDriver
    - Supports Page Object patterns
    - Integrated with popular .NET testing tools and frameworks






