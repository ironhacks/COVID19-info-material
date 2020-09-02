<h3 align=center> COVID-19 Data Science Challenge August 2020</h3>
<h4 align=center> Guidelines for Reading your Dashboard for Phase 1</h4>



In your dashboard, we report a selected set of metrics related to your model's **prediction accuracy** related to the `sum_visit_counts` of a set of unique uuids for a particular week (week 18 to week 21 well as your **effort** in achieving this accuracy.

Your dashboard has two components: Your scores and Your peers.

- The `Your scores` tab tells you about individual metrics.
- The `Your peers` tab provide you more insight into your current standing in the hack. Please not that the mean and the standard deviation are based on the number of submission during this particular phase! 

In both components, we present the following metrics: 

| Metric            | Brief Description/Formula                                    | Data type                     |
| :---------------- | ------------------------------------------------------------ | ----------------------------- |
| `MSPE`            | The Mean Squared Prediction Error for the `sum_visit_counts` for a certain week (e.g. `week 19`) is calculated with this [formula](https://raw.githubusercontent.com/ironhacks/COVID19-info-material/master/MSPE.png) with n being the unique `uuids`  in the week for which you are forecasting for (e.g.week 19); if your cells where "empty" for certain `uuids` we assume that you submitted a `0`; the lower your MSPE, the better your model; please note that the MSPE is sensitive to outliers. The MSPE is commonly used in other Data Science Challenges; thus, in this challenge, we will be using the MSPE | FLOAT (rounded to two digits) |
| `MAPE`            | The Mean Absolute Prediction Error for the `sum_visit_counts` for a certain week (e.g.`week 19'`) is calculated with this [formula](https://raw.githubusercontent.com/ironhacks/COVID19-info-material/master/MAPE.png); with n being the number of unique `uuids`  in the week that you are forecasting for (e.g. week 19); if your cells where "empty" for certain `uuids` we assume that you submitted a `0`; the lower your MAPE, the better your model | FLOAT (rounded to two digits) |
| `Notebook Effort` | The `Notebook Effort` score describes your effort in using your notebook to build your model; it considers the number of cells as well as your activity in modifying and running them. The higher your metric the better! | INTEGER                       |
| `BigQuery Effort` | The `BigQuery Effort` describes your effort in understanding the data we provided you; it considers the number and the nature of the jobs you launched via your notebook. The higher your metric the better! | INTEGER                       |

> How to read your scores and your peers? Here some tips:
>
> - The lower your MSPE the better; however, you do not necessarily need to have a value close to 0 to win the hack. Make sure you also compare the mean and the standard deviation in the `your peers` tab; 
> - Your standing relative to the mean tells you how you are performing compared to the mean! Also, note that a large distance between you and the mean does not mean that you cannot catch up (or the other way around); we will eventually rank-order all participants to select the Best Solutions. 
> - Your Big Query Effort and your Notebook Effort count towards your overall effort during the hack. To allocate improvement spirit incentives we will consider both - your MSPE as well as your effort
>
> And a final note: Only the TWO best submissions will be considered for the final MSPE and MAPE calculation! And do not forget: According to the rules of the challenge, only 2 submissions are needed to qualify for an award. 



