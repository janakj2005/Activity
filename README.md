# Activity - 06-10-2026


## Testing Code

```
from selenium import webdriver
from selenium.webdriver.common.by import By
from selenium.webdriver.support.ui import Select
import time
driver=webdriver.Chrome()

driver.get("https://vinothqaacademy.com/demo-site/")
driver.find_element(By.ID,"vfb-5").send_keys("Saranya")
driver.find_element(By.ID,"vfb-7").send_keys("Selvam")
female=driver.find_element(By.ID,"vfb-31-2")
female.click()
selenium=driver.find_element(By.ID,"vfb-20-0")
selenium.click()
java=driver.find_element(By.ID,"vfb-20-1")
java.click()
driver.find_element(By.ID,"vfb-13-address").send_keys("13,kulathankarai street")
driver.find_element(By.ID,"vfb-13-address-2").send_keys("kulakarai st")
driver.find_element(By.ID,"vfb-13-city").send_keys("13")
driver.find_element(By.ID,"vfb-13-city").send_keys("vellore")
driver.find_element(By.ID,"vfb-13-zip").send_keys("632007")
state = driver.find_element(By.ID, "vfb-13-state")
state.send_keys("Tamil Nadu")
country = Select(
    driver.find_element(By.ID, "vfb-13-country")
)
country.select_by_visible_text("India")
driver.find_element(By.ID,"vfb-14").send_keys("saranya@gmail.com")
driver.find_element(By.ID,"vfb-18").send_keys("08/09/2025")
hour = Select(
    driver.find_element(By.ID, "vfb-16-hour")
)
hour.select_by_visible_text("10")
minute = Select(
    driver.find_element(By.ID, "vfb-16-min")
)
minute.select_by_visible_text("30")
driver.find_element(By.ID,"vfb-19").send_keys("9880109821")
query = driver.find_element(By.ID, "vfb-23")
query.send_keys("I am interested in Selenium automation training.")
time.sleep(5)
driver.quit()
```
