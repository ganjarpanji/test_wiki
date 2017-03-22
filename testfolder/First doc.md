# MedicationCoach ( No State )

- sends reminder at every morning, afternoon, evening, if there is any medication needs to be taken.
- sends reminder right after meal time input, if the meal time input is close to the current time.
- sends summary of medications taken/not taken at 9:00 every day, if the user took medication properly.

## Native Components

### MedicationCoachStream

```swift
class MedicationCoachStream {
  
  class MedicationGoal {  
    let name : String
    let dose : String
    let timeSlot : Array<Array<String>> [["9:00","12:00"],["12:00","17:00"],["17:00","23:00"]]
    let dayOfWeek: Array<Int> // Monday:0, Tuesday:1, .., Sunday:6
  }
}
```