## Concepts
* **Task**: A thing to be done. Has several attributes beyond the automatic (name, description etc.)
  * **Date**: The date on which the task should be started. Used to determine if the task fits within a given timeframe.
  * **Due date**: Date by which the task should be finished. Not used in deterining tasks' pool or timeframe.
  * **Start date**: The day on which the task is planned to be performed.
* **Pool**: Tasks are divided into groups based on certain criteria (see below).
* **Timeframe**: Configurable span of time (in days) used to plan tasks.

## Pools
* **Undated**: Tasks without a date set.
* **Future**: Tasks with the date beyond current timeframe.
* **Current**: Tasks who's date has arrived or passed.
* **Planned**: Tasks that have been assigned a start date.

## Workflow
1. When a task is created, it is assigned a date. Assuming the date is in the future beyond current timeframe, the task shows up in the "Future" pool.
2. When the task's date arrives within the timeframe, the task appears in the "Current" pool.
3. The user moves tasks from the "Current" pool into each of the days of the timeframe.
4. Any task that isn't completed when the day has passed, goes back into the "Current" pool to be re-assigned a new day.
