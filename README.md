Установка playwright:
1) pip install pytest-playwright
2) playwright install

<details>
    <summary>Основные действия:</summary>
    
```python
    get_started = page.get_by_role("link", name="Get started")
    get_started.click()
    
    page.get_by_role("link", name="Get started").click()
```
    
locator.check()	-- Check the input checkbox  
locator.click() --	Click the element  
locator.uncheck() --	Uncheck the input checkbox  
locator.hover() --	Hover mouse over the element  
locator.fill() --	Fill the form field, input text  
locator.focus() --	Focus the element  
locator.press() --	Press single key  
locator.set_input_files() --	Pick files to upload  
locator.select_option() --	Select option in the drop down  
</details> 


<details>
    <summary>Проверки:</summary>  
    
```python
import re
from playwright.sync_api import expect

expect(page).to_have_title(re.compile("Playwright"))
```

expect(locator).to_be_checked() --	Checkbox is checked  
expect(locator).to_be_enabled() --	Control is enabled  
expect(locator).to_be_visible() --	Element is visible  
expect(locator).to_contain_text() --	Element contains text  
expect(locator).to_have_attribute() --	Element has attribute  
expect(locator).to_have_count() --	List of elements has given length  
expect(locator).to_have_text() --	Element matches text  
expect(locator).to_have_value() --	Input element has value  
expect(page).to_have_title() --	Page has title  
expect(page).to_have_url() --	Page has URL 
</details> 