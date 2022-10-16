# fnwork
Mine
ChromeDriver driver = new ChromeDriver();
DevTools devTools = driver.getDevTools();
devTools.createSession();
devTools.send(Emulation.setGeolocationOverride(Optional.of(52.5043),
                                               Optional.of(13.4501),
                                               Optional.of(1)));
driver.get("https://my-location.org/");
driver.quit()
