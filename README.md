# Selenium grid

0. Install `selenium-webdriver` node package [need to setup package.json]
1. Start hub
    java -jar selenium-server-standalone-2.45.0.jar -role hub
2. Start [many] phantom instances
    phantomjs --webdriver=8910 --webdriver-selenium-grid-hub=http://localhost:4444
3. Run test
    node index.js