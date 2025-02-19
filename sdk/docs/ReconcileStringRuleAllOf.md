

# ReconcileStringRuleAllOf


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**comparisonType** | [**ComparisonTypeEnum**](#ComparisonTypeEnum) | The available values are: Exact, Contains, CaseInsensitive, ContainsAnyCase, IsOneOf | 
**oneOfCandidates** | **Map&lt;String, List&lt;String&gt;&gt;** | For cases of \&quot;IsOneOf\&quot; a set is required to match values against.  Fuzzy matching of strings against one of a set. There can be cases where systems \&quot;A\&quot; and \&quot;B\&quot; might use different terms for the same logical entity. A common case would be  comparison of something like a day count fraction where some convention like the \&quot;actual 365\&quot; convention might be represented as one of [\&quot;A365\&quot;, \&quot;Act365\&quot;, \&quot;Actual365\&quot;] or similar.  This is to allow this kind of fuzzy matching of values. Note that as this is exhaustive comparison across sets it will be slow and should therefore be used sparingly. |  [optional]
**appliesTo** | [**AggregateSpec**](AggregateSpec.md) |  | 
**ruleType** | [**RuleTypeEnum**](#RuleTypeEnum) | The available values are: ReconcileNumericRule, ReconcileDateTimeRule, ReconcileStringRule, ReconcileExact | 



## Enum: ComparisonTypeEnum

Name | Value
---- | -----
EXACT | &quot;Exact&quot;
CONTAINS | &quot;Contains&quot;
CASEINSENSITIVE | &quot;CaseInsensitive&quot;
CONTAINSANYCASE | &quot;ContainsAnyCase&quot;
ISONEOF | &quot;IsOneOf&quot;



## Enum: RuleTypeEnum

Name | Value
---- | -----
RECONCILENUMERICRULE | &quot;ReconcileNumericRule&quot;
RECONCILEDATETIMERULE | &quot;ReconcileDateTimeRule&quot;
RECONCILESTRINGRULE | &quot;ReconcileStringRule&quot;
RECONCILEEXACT | &quot;ReconcileExact&quot;



