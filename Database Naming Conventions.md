## MsSQL / MySQL

#### Table Name
- We use **singular** names and our notation is **PascalCase**. (e.g. `User`, `Product`, `Role`)

#### Column Name
- We use **singular** names and our notation is **PascalCase**. (e.g. `FirstName`, `Amount`)

#### Stored Procedure Name
- Use the prefix `usp_`, names will be **singular** and notation **PascalCase**. Stored Procedure name format should be `usp_[Object][Action]`. (e.g. `usp_UserAdd`, `usp_UserDelete`)

> Don’t use the prefix `sp_` in the stored procedure name, because SQL Server always looks for a stored procedure beginning with “sp_” in the following order: the master database, the stored procedure based on the fully qualified name provided, the stored procedure using dbo as the owner, if one is not specified.

#### View Name
- Use the prefix `vw_`, names will be **singular** and notation **PascalCase**. View name format should be `vw_[ViewName]`. (e.g. `vw_UserDetail`, `vw_ProductDetailList`)

#### Trigger Name
- Use the prefix `trg_`, names will be **singular** and notation **PascalCase**. Trigger name format should be `trg_[TableName][ActionName]`. (e.g. `trg_User_AfterInsert`)

#### Function Name
- Use the prefix `fn_`, names will be **singular** and notation **PascalCase**. Function name format should be `fn_[FunctionName]`. (e.g. `fn_FormatDate`)

#### Primary Key Column Name
- Use `Id` without table name. Regardless of the name of your table, the primary key name must be `Id`.

#### Foreign Key Column Name
- FK column name format should be `[TargetTableName][TragetPrimayKeyName]` and notation **PascalCase**. (e.g. `UserId`)

#### Foreign Key Name
- Use the prefix `FK_`, names will be **singular** and notation **PascalCase**. FK name format should be `FK_[TableName][RelatedTableName]`. (e.g. `FK_User_Role`)
