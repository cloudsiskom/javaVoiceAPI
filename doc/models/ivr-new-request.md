
# IVR New Request

## Structure

`IVRNewRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Action` | `String` | Required | - | String getAction() | setAction(String action) |
| `IvrName` | `String` | Required | - | String getIvrName() | setIvrName(String ivrName) |
| `IvrTitle` | `String` | Required | - | String getIvrTitle() | setIvrTitle(String ivrTitle) |
| `Lang` | `String` | Required | - | String getLang() | setLang(String lang) |
| `Gender` | `String` | Required | - | String getGender() | setGender(String gender) |
| `AnnauncementText` | `String` | Required | - | String getAnnauncementText() | setAnnauncementText(String annauncementText) |
| `MaxTrying` | `String` | Required | - | String getMaxTrying() | setMaxTrying(String maxTrying) |
| `ExitKey` | `String` | Required | - | String getExitKey() | setExitKey(String exitKey) |
| `BackMenu` | `String` | Required | - | String getBackMenu() | setBackMenu(String backMenu) |
| `MainMenu` | `String` | Required | - | String getMainMenu() | setMainMenu(String mainMenu) |
| `KeyPressed` | `String` | Required | - | String getKeyPressed() | setKeyPressed(String keyPressed) |
| `IvrParent` | `String` | Required | - | String getIvrParent() | setIvrParent(String ivrParent) |
| `IvrAction` | `String` | Required | - | String getIvrAction() | setIvrAction(String ivrAction) |

## Example (as JSON)

```json
{
  "action": "[ACTION]",
  "ivr_name": "[IVR_NAME]",
  "ivr_title": "[IVR_TTITLE]",
  "lang": "[LANG]",
  "gender": "[GENDER]",
  "annauncement_text": "[TEXT_TO_SPEECH]",
  "max_trying": "[MAX_TRYING]",
  "exit_key": "[EXIT_KEY]",
  "back_menu": "[BACK_MENU]",
  "main_menu": "0",
  "key_pressed": "[KEY_PRESSED]",
  "ivr_parent": "[PARENT_IVR_ID]",
  "ivr_action": "NONE"
}
```

