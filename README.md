Due to chrome's preview method, it doesn't download the pdf while running `selenium-side-runner`

In order to download the pdf using `selenium-side-runner` use the following command
```
selenium-side-runner -c '{
  "capabilities": {
    "goog:chromeOptions": {
      "extensions": ["path/to/disable_download_bar.crx"]
    }
  }
}' download-pdf.side

```
