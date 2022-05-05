<!-- 220328.094653 -->

<h1 align="center">

  <img src="../resource/image/logo/MAWS-logo-512x350.png" alt="MyAvatool Web Service logo" width="256">
  <br>
  Development notes
  <br>
  <br>

</h1>





























## Exception closed dispensing

### Process
* Fast Dose Dispensing form
* Get the content of the Dispense History field
* Get the historical dates
* Loop through the historical dates and see if any match the Dispense Date
  * All dates, or a specific number of dates?
* If yes, error
  * If no, continue

Dispensing History field = scrolling text field (10008)
Dispensing Date field = date field (10007)




## Christine's request
* Admission (Outpatient)
* Choose a PA episode > Edit
* If the Preadmit/Admission date is empty, don't do anything
* If the Preadmit/Admission date == system date, don't do anything
* If the Preadmit/Admission date != system date:
  * Warn user to modify date
  * Warn again!

### Test plan
*

