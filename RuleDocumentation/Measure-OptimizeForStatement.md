# ForStatementCanBeImproved
**Severity Level: Information**

## Description
The way to write a For loop can speed it up performance of a script 
See: http://www.old.dougfinke.com/blog/index.php/2011/01/16/make-your-powershell-for-loops-4x-faster/

## How to Fix
Change the position property.

## Example
### To improve ：
```PowerShell
   $Range=1..10
   For($i=0; $i -lt $Range.Count; $i++) { $i }
```

### Improved:
```PowerShell
   $Range=1..10
   $RangeCount = $Range.Count
   For($i=0; $i -lt $RangeCount; $i++) { $i }
```

### Function :   OptimizationRules\Measure-OptimizeForStatement
