# Hey ✌

Rodrigo Magalhães' Portfolio
About Me
Hello! I'm Rodrigo Magalhães, a 31-year-old Junior QA Analyst in training, living in Ninheira, Minas Gerais - Brazil.
I have a degree in Accounting and completed a Quality Assurance bootcamp at TripleTen in 2025. After 13 years
as an Administrative Assistant in a city hall, where I honed my analytical and organizational skills, I'm transitioning
to technology, focusing on software testing and automation, including the use of JavaScript for automated testing.
I'm fluent in Spanish, have basic English, and am motivated to contribute to agile teams.

## Contact e Links

| Type | details |
| :---: | :--- |
| 📧 **E-mail** | rodrovisk@gmail.com |
| 📞 **Telefone** | +55 (38) 99923-9610 |
| 🔗 **LinkedIn** | [rodrigo-magalhães-b02628205](https://www.linkedin.com/in/rodrigo-magalhães-b02628205) |
| ⚙️ **GitHub** | [rodrovisk94](https://github.com/rodrovisk94) |

| Skills | Tools & Soft Skills |
| :---: | :---: |
| JavaScript | Communication |
| Figma | Postman |
| Jira | Resilience |
| VS Code | Cypress |
| Git | Multiculturalism |
| HTML5 | Leadership |
| CSS3 | Creativity |
| Python | Commitment |
| Docker | k6 |
| Selenium | Jenkins |

 💻cod Javascript:

## My cod (Test Login with Selenium and JS)

```javascript
const { Builder, By, until } = require('selenium-webdriver');

async function loginTest() {
    let driver = await new Builder().forBrowser('chrome').build();
    try {
        await driver.get('[https://example.com/login](https://example.com/login)');
        await driver.findElement(By.id('username')).sendKeys('testuser');
        await driver.findElement(By.id('password')).sendKeys('testpass');
        await driver.findElement(By.id('login-btn')).click();
        await driver.wait(until.elementLocated(By.id('welcome')), 5000);
        console.log('Login bem-sucedido!');
    } finally {
        await driver.quit();
    }
}

loginTest();
     
