
# Create Intent Request

## Structure

`CreateIntentRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `AiName` | `String` | Required | - | String getAiName() | setAiName(String aiName) |
| `DisplayName` | `String` | Required | - | String getDisplayName() | setDisplayName(String displayName) |
| `TrainingPhrases` | `String` | Required | - | String getTrainingPhrases() | setTrainingPhrases(String trainingPhrases) |
| `MessageTexts` | `String` | Required | - | String getMessageTexts() | setMessageTexts(String messageTexts) |

## Example (as JSON)

```json
{
  "ai_name": "[AI_NAME]",
  "display_name": "[DISPLAY_NAME",
  "training_phrases": "[TRAINING_PHRASE,SPARATED BY ;]",
  "message_texts": "[RESPONSE_TEXT SPARATED BY ;]"
}
```

