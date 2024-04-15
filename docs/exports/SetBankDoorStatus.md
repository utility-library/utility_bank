# SetBankDoorStatus
Sets the status of a bank door.

| Argument | Data Type | Nedeed                           | Default | Description                                                                                            |
|----------|-----------|----------------------------------|---------|--------------------------------------------------------------------------------------------------------|
| `bankId` | number    | :material-checkbox-blank-circle: | `-`     | The index in the Config.Banks table                                                                    |
| `doorId` | string    | :material-checkbox-blank-circle: | `-`     | Internal id to refer the door, generally can be one of the following values: vault, prevault, shutters |
| `status` | boolean   | :material-checkbox-blank-circle: | `-`     | True to open the door, false to close it (for shutters its inverted, so true = closed)                 |

---

??? example
    ```
    exports["utility_bank"]:SetBankDoorStatus(1, "shutters", true)
    ```