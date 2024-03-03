Due to chrome's download preview feature, it doesn't download the pdf while running `selenium-side-runner`

In order to download the pdf using `selenium-side-runner` use the following command
```
selenium-side-runner -c '{
  "capabilities": {
    "goog:chromeOptions": {
      "prefs": {
        "download.prompt_for_download": false
      }
    }
  }
}' download-pdf.side


```
