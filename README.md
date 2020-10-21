# SeleniumBrowser_proxy
Methods to load the SeleniumBrowser with proxy faster

## Install Selenium WebDrivers for web crawling

In order to use Selenium, you have to install a few drivers for web crawling. 

### MacOSX

If you're using MacOSX like I am, you will need to do the following:

First of all, you need Homebrew.
**If you don't have Homebrew**, click [here](https://brew.sh), or just do the following:

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```

**If you're behind a proxy and can't install Homebrew**, first configure your git proxy settings:
```
git config --global http.proxy http://{PROXY_HOST}:{PORT}
```
Replace your {PROXY_HOST} and your {PORT}.

Then install homebrew using proxy settings as well:
```
/bin/bash -c "$(curl -x {PROXY_HOST}:{PORT} -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```
And finally alias `brew` so it always uses your proxy settings:

```
alias brew="https_proxy={PROXY_HOST}:{PORT} brew"
```

**Now that you have homebrew:**

#### Install geckodriver (firefox) for Seleium WebDriver library (MacOSX)

```
brew install geckodriver
```

#### Install chromedriver (GoogleChrome) for Seleium WebDriver library (MacOSX)

```
brew install chromedriver
```

#### Install phantomjs (headless *no display* simulator) for Seleium WebDriver library (MacOSX)

```
brew install phantomjs
```

### Ubuntu

Ubuntu geckodriver installation
https://askubuntu.com/questions/870530/how-to-install-geckodriver-in-ubuntu

Ubuntu chromedriver installation
https://gist.github.com/ziadoz/3e8ab7e944d02fe872c3454d17af31a5
