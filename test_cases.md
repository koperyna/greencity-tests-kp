# Test Case №1: Verify interface language switch functionality

**Preconditions:**

* User is on the GreenCity Events page (https://www.greencity.cx.ua/#/greenCity/events)
* Language switcher is available on the page
* Default language is set (Ukrainian)

| Step | Action                   | Data            | Expected Result                                     |
| ---- | ------------------------ | --------------- | --------------------------------------------------- |
| 1    | Open Events page         | URL             | Page loads in default language                      |
| 2    | Locate language switcher | -               | Language selector is visible                        |
| 3    | Open language dropdown   | -               | List of available languages is displayed            |
| 4    | Select another language  | English         | Page reloads OR updates dynamically                 |
| 5    | Observe UI text          | -               | All visible UI elements change to selected language |
| 6    | Check main elements      | Titles, buttons | Text is translated correctly                        |
| 7    | Navigate within page     | Click event     | Selected language persists                          |
| 8    | Refresh page             | -               | Selected language is persisted                      |

# Test Case №2: Verify date filter functionality using date picker

**Preconditions:**

* User is on the GreenCity Events page (https://www.greencity.cx.ua/#/greenCity/events)
* Events list contains items with different dates
* Date filter (calendar picker) is available


| Step | Action                 | Data            | Expected Result                             |
| ---- | ---------------------- | --------------- | ------------------------------------------- |
| 1    | Open Events page       | URL             | Page loads successfully                     |
| 2    | Locate date filter     | -               | Date picker input is visible                |
| 3    | Click on date input    | -               | Calendar dropdown opens                     |
| 4    | Select a specific date | 04.02.2026      | Calendar closes and date is applied         |
| 5    | Observe events list    | -               | Only events for selected date are displayed |
| 6    | Verify event dates     | -               | All shown events match selected date        |
| 7    | Clear or change date   | another date    | Events list updates accordingly             |

## Negative Scenario: Invalid interaction

| Step | Action                 | Data | Expected Result               |
| ---- | ---------------------- | ---- | ----------------------------- |
| 1    | Open calendar          | -    | Calendar appears              |
| 2    | Click outside calendar | -    | Calendar closes               |
| 3    | Do not select date     | -    | Filter is not applied         |
| 4    | Observe events         | -    | Events list remains unchanged |


# Test Case №3: Verify navigation to event details page

**Preconditions:**

* User is on the GreenCity Events page (https://www.greencity.cx.ua/#/greenCity/events)
* At least one event exists

| Step | Action              | Data | Expected Result                         |
| ---- | ------------------- | ---- | --------------------------------------- |
| 1    | Click on event card | -    | User is redirected                      |
| 2    | Observe URL         | -    | URL changes to event details page       |
| 3    | Check page content  | -    | Full event details are displayed        |
| 4    | Verify consistency  | -    | Data matches preview from previous page |

