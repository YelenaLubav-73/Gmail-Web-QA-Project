# Bug ID: BUG_003
## Title:          Language dropdown width dynamically resizes according to the selected language, causing truncation of longer language names. 
** Related Test Case: ** TC-GUI-003
** Requirement ID: ** GUI-7.1, GUI-7.2, GUI-7.3

## Environment :

### Desktop:
- OS: Windows 10, macOS Sonoma 14.6.1
- Browsers: Google Chrome, Microsoft Edge, Mozilla Firefox

### Mobile:
- OS: iOS
-Browsers: Safari, Chrome (iOS)

**Devices:** Windows Laptop, Mac Pro, iPhone 12 Pro Max
 
## Precondition:
The Gmail authorization page is open.
The language selection dropdown is available.

## Steps to Reproduce:
Step 1: 
Select a language with a short name (e.g., "Suomi" or "eesti"); 
Step 2: 
Reopen the language dropdown and observe language options with long names (e.g., "English (United States)"). 

## Expected Result 1:
The language selection dropdown expands to an appropriate width. All language options are fully visible, readable, and not truncated.

## Actual Result 1:
On desktop browsers (Chrome, Edge, and Firefox), the dropdown width is adjusted to the selected language, causing truncation of longer language names.
On mobile browsers (Safari and Chrome), all language names were fully visible and readable.

## Expected Result 2:
The language selection dropdown remains fully expanded. All language names are displayed completely, without clipping or truncation.

## Actual Result 2:
On desktop browsers (Chrome, Edge, and Firefox), long language names were truncated and not fully visible. 
On mobile browsers (Safari and Chrome), the dropdown expanded correctly and all language names remained fully visible and readable.

## Observation:
Reproduced on desktop browsers on Windows and macOS; not reproduced on mobile browsers (iOS).

## Recommendation:
Review the dropdown rendering behavior in desktop browsers. 

Severity:   Low
Priority:     Low
Status:     Open 
Reported by: Yelena Lubavin

