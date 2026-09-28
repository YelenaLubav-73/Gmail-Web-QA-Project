# Bug ID: BUG_003
## Title: Language dropdown width dynamically resizes according to the selected language, causing truncation of longer language names. 
**Related Test Case:** TC-GUI-003
**Requirement ID:** GUI-7.1, GUI-7.2, GUI-7.3

## Environment:

### Desktop:
- OS: Windows 10, macOS Sonoma 14.6.1
- Browsers: Google Chrome, Microsoft Edge, Mozilla Firefox

### Mobile:
- OS: iOS
- Browsers: Safari, Chrome (iOS)

**Devices:** Windows Laptop, Mac Pro, iPhone 12 Pro Max
 
## Precondition:
- The Gmail authorization page is open.
- The language selection dropdown is available.

## Steps to Reproduce:
### Step 1: 
- Select a language with a short name (e.g., "Suomi" or "eesti"); 
### Step 2: 
- Reopen the language dropdown and observe language options with long names (e.g., "English (United States)"). 

## Expected Result 1:
- The language selection dropdown expands to an appropriate width. All language options are fully visible, readable, and not truncated.

## Actual Result 1:
- On desktop browsers (Chrome, Edge, and Firefox), the dropdown width is adjusted to the selected language, causing truncation of longer language names.
- On mobile browsers (Safari and Chrome), all language names were fully visible and readable.

## Expected Result 2:
- The language selection dropdown remains fully expanded. All language names are displayed completely, without clipping or truncation.

## Actual Result 2:
- On desktop browsers (Chrome, Edge, and Firefox), long language names were truncated and not fully visible. 
- On mobile browsers (Safari and Chrome), the dropdown expanded correctly and all language names remained fully visible and readable.

## Observation:
Reproduced on desktop browsers on Windows and macOS; not reproduced on mobile browsers (iOS).

## Recommendation:
Review the dropdown rendering behavior in desktop browsers. 

**Severity:** Low  
**Priority:** Low  
**Status:** Open  
**Reported by:** Yelena Lubavin

---

# Bug ID: BUG_004
## Title: Month names are truncated in the registration dropdown list on high-DPI displays 
**Related Test Case:** TC-GUI-005
**Requirement ID:** GUI-1.1, GUI-1.2

## Environment:

- **OS:** Windows 10
- **Device:** ASUS UX310U Laptop
- **Screen Resolution:** 1920×1080
- **Display Scale:** 175%
- **Browser Zoom:** 100%
- **Browser Window:** Full Screen
- **Browsers:** Microsoft Edge, Google Chrome

## Precondition:
- Navigate to the "Basic Information" registration page by completing the previous registration step and clicking the "Next" button.

## Steps to Reproduce:

### Step 1:
- Open the "Month" dropdown list on the "Basic Information" registration page.
### Expected Result 1:
- The "Month" dropdown list is opened and displayed correctly.
### Actual Result 1:
- The "Month" dropdown list is opened.

### Step 2:
- Inspect the displayed month names.
### Expected Result 2:
- All month names are fully visible and readable without truncation.
### Actual Result 2:
- One or more month names in the dropdown list are truncated and not fully readable.  

## Observation:
The issue was reproduced in Microsoft Edge and Google Chrome on an ASUS UX310U laptop running Windows 10 with display scaling set to 175% and browser zoom set to 100%. The issue was observed in both English and Russian versions of the registration form.

**Severity:** Low  
**Priority:** Low  
**Status:** Open  
**Reported by:** Yelena Lubavin

