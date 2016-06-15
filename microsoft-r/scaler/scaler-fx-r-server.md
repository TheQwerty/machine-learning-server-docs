---

# required metadata
title: "RevoScaleR Functions"
description: "ScaleR Functions"
keywords: "RevoScaleR, ScaleR"
author: "j-martens"
manager: "Paulette.McKay"
ms.date: "06/13/2016"
ms.topic: "article"
ms.prod: "microsoftr"
ms.service: ""
ms.assetid: ""

# optional metadata
ROBOTS: ""
audience: ""
ms.devlang: ""
ms.reviewer: ""
ms.suite: ""
ms.tgt_pltfrm: ""
ms.technology: ""
ms.custom: ""

---

# ScaleR Function Map for Microsoft R Server

The `RevoScaleR` package includes hundreds of functions you can use for data analysis, for high-performance and distributed computing, and more. About 180 functions can be called directly from the command-line.

This topic is specific to Microsoft R Server. Here you can learn about the most commonly used functions for Microsoft R Server users.  

You can also learn about the functions recommended for these editions:
+ Microsoft R Client
+ Microsoft R Server for Hadoop
+ Microsoft R Server for Teradata
+ [SQL Server R Services](functions-for-sql-server-data.md)



## Functions for Data Analysis

| |![import](../media/scaler-puzzle1.png)|![import](../media/scaler-puzzle2.png)|![import](../media/scaler-puzzle3.png)|![import](../media/scaler-puzzle4.png)|  
|-----------------------|-----------------------|-----------------------|-----------------------|-----------------------|
|                       |**Import / Export**    |**Manipulate / Clean / Transform**|**Visualize**          |**Analyze / Learn / Predict**    |
|**Most Popular <br />Functions**  |<!--COL-1-->[`rxImport()`]() <br /> [`rxXdfToText()`]() <br /> [`rxGetInfo()`]() <br /> [`rxSetInfo()`]() <br /> [`rxGetVarInfo()`]() <br /> [`rxSetVarInfo()`]() <br /> [`rxGetVarNames()`]() <br /> [`rxCompressXdf()`]() <br /> [`RxXdfData()`]()<br />[`RxTextData()`]() <br /> [`RxSasData()`]() <br /> [`RxSpssData()`]() <br /> [`RxOdbcData()`]() <br /> [`RxSqlServerData()`](RxSqlServerData.md) <br />[`RxTeradata()`]() <br />[`rxOpen()`](rxOpen.md) <br />[`rxClose()`](rxClose.md)  <br />[`rxReadNext()`](rxReadNext.md) <br /> [`rxSetFileSystem()`]() <br /> [`rxGetFileSystem()`]() <br />[`RxHdfsFileSystem()`]() <br /> [`RxNativeFileSystem()`]() <br /><br />  Functions `rxDataStep()`,<br/> `rxXdfToDataFrame()`, <br/>and `rxReadXdf:Reads()`<br/> can also read <br/>an .XDF file into <br/>a data  frame.|<!--COL-2--> [`rxDataStep()`]() <br /> [`rxFactors()`]() <br /> [`rxSort()`]() <br /> [`rxMerge()`]() <br /> [`rxSplit()`]() <br /> [`rxExecuteSQLDDL()`](rxExecuteSQLDDL.md)<br /> |<!--COL-3--> [`rxHistogram()`]() <br />[`rxLinePlot()`]() <br /> [`rxLorenz()`]()  <br /> [`rxRocCurve()`]()|<!--COL-4-->_Descriptive Statistics <br/>& Cross-Tabulation:_ <br /> [`rxSummary()`]() <br /> [`rxQuantile()`]() <br /> [`rxCrossTabs()`]() <br /> [`rxCube()`]() <br /> [`rxMarginals()`]()  <br /> [`rxChiSquaredTest()`]() <br /> [`rxFisherTest()`]() <br /> [`rxKendallCor()`]() <br /> [`rxPairwiseCrossTab()`]() <br /> [`rxRiskRatio()`]() <br /> [`rxOddsRatio()`]() <br /> <br /> _Statistical Modeling:_ <br /> [`rxLinMod()`]() <br /> [`rxCovCor()`]() <br />[`rxCov()`]() <br /> [`rxCor()`]()  <br /> [`rxSSCP()`]() <br />[`rxLogit()`]() <br /> [`rxRoc()`]()  <br /> [`rxGlm()`]() <br />[`rxDTree()`]() <br /> [`rxKmeans()`]()  <br /> [`rxDForest()`]() <br /> <br /> _Prediction:_ <br /> [`rxPredict()`]() |
|**Less Used <br />Functions**  |<!--COL-1--> [`RxNativeFileSystem()`]() |<!--COL-2--> [`rxDataStep()`]() <br /> [`rxFactors()`]()|<!--COL-3--> [`rxHistogram()`]()|<!--COL-4--> Something |

>[!IMPORTANT]
>This is not an exhaustive list of functions in the RevoScaleR package. If you want to see the entire set of functions,  [follow these steps.](#findmore)



<br>
## Other Functions 

|![import](../media/scaler-data.png)  |![import](../media/scaler-context.png)| ![import](../media/scaler-utility.png)| ![import](../media/scaler-utility.png)|  
|----------------------------------------|--------------------------------------|--------------------------------------|--------------------------------------|
|**Data Sources**                        |**Compute Context**                 |**Utility Functions**                 |**High Performance / Distributed Computing**  |
|<!--COL-1--> [`()`]() <br /> [`()`]() <br /> [`()`]() <br /> [`()`]() <br /> [`()`]() <br /> [`()`]() <br /> [`()`]() <br /> [`()`]() <br /> [`()`]() <br /> [`()`]() <br /> [`()`]() <br /> [`()`]() <br /> [`()`]() <br /> [`()`]() <br /> [`()`]() <br /> [`()`]()|<!--COL-2-->  |<!--COL-3--> [`rxOptions()`]()<br /> [`rxGetOption()`]() <br /> [`rxRngNewStream()`]() <br /> [`rxRngDelStream()`]() <br /> [`rxRngGetStream()`]() <br /> [`rxRngSetStream()`]() <br /> [`rxGetEnableThreadPool()`]() <br /> [`rxSetEnableThreadPool()`]()  <br /> [`rxStepControl()`]()  |<!--COL-4--> [`RxComputeContext()`](RxComputeContext.md) <br /> [`RxForeachDoPar()`]() <br /> [`RxLocalParallel()`]() <br /> [`RxLocalSeq()`]() <br /> [`rxGetComputeContext()`](rxGetComputeContext.md) <br /> [`rxSetComputeContext()`](rxSetComputeContext.md) <br /> [`RxInSqlServer()`](RxInSqlServer.md) |



<br>
[`rxIsOpen()`](rxIsOpen.md)
[`rxSqlServerDropTable()`](rxSqlServerDropTable.md)     
[`rxSqlServerTableExists()`](rxSqlServerTableExists.md)
[`rxWriteNext()`](rxWriteNext.md)
<br>


<a name="findmore"></a>
##See All Functions and Help Files

Get the set of public functions and see the associated help pages using the following steps.

**To see the `RevoScaleR` functions that can be called from the commands-line:**

1. With Microsoft R Server or R Client installed, launch an R console with `Rgui.exe`, R Tools for Visual Studio, RStudio, or another IDE. 

1. In the console, return the number of objects by typing the following at the R prompt `>`:
   ```
   > search()
   ```

1. Identify the position of the object you are interested in. In the case of our example, RevoScaleR is in the fifth position.

1. At the R prompt, type `objects(<position>)` to reveal the set of functions such as:
   ```
   > objects(5)
   ```

   ![objects](../media/scaler-rconsole-obj.png)

1. At the R prompt, type `?<function_name>` to open the help file for that function, such as:
   ```
   > ?rxXdfData
   ```