### Requirements:
UiPath.Web.Activities v1.4.4

### Config

| Parameter  | Description  |
| ------------ | ------------ |
| orchestratorURL  | orchestrator's url  |
| organizationUnit  | 0 - orchestrator hasn't organization units, any other digit will be organization unit ID  |
| tenancyName | Login credentials  |
| userName | Login credentials  |
| passWord  | Login credentials  |
| startDate  | First date of range  |
| endDate  | Last date of range  |
| jobsList  | List of jobs that robot will collect. Comma (,) is delimiter.  |
| writeTo  | 0 - CSV, 1 - XLSX  |
| timeShift  | Difference in time zones. Robot will shift output times on that value. Positive and negative numbers allowed  |


### Workflow

Fill in config file.
Run.
Robot will save excel table called by release name and current date time with jobs time in Files folder.
Errors will be saved in Data/Errors.xlsx if any.