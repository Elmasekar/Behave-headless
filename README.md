# How to run browser in headless mode in Behave on [LambdaTest](https://www.lambdatest.com/?utm_source=github&utm_medium=repo&utm_campaign=Behave-headless)

If you want to run a browser in headless mode for an automation test in Behave on Lambdatest, you can use the following steps. You can refer to sample test repo [here](https://github.com/LambdaTest/Python-Behave-Selenium).

# Steps:

You can run a test in headless mode by providing it as a capability in `config.json` file. The `config.json` would look something like this:

 ```python
 [
	{
		"platform": "Windows 10",
		"browserName": "chrome",
		"version": "latest",
		"build": "Behave Selenium Sample",
		"name": "Behave Sample Test",
		"headless"  :  True
	}
]

 ```
 
* Full documentation for configuration [Behave](https://behave-webdriver.readthedocs.io/en/latest/quickstart.htmll).
## Run your test

### Running tests through local (linux/unix)
```bash
paver run 
```
###Running tests through local (windows)
```bash
behave features/test.feature 
```

### Running tests through jenkins
```bash
paver run jenkins
```

# Links:

[LambdaTest Community](http://community.lambdatest.com/)


