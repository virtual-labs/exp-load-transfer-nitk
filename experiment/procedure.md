<u>**Aim of the experiment: Load Transfer from one Feeder to other during Transformer Maintenance**</u>

Whenever Transformer is to be taken out for service maintenance, the corresponding circuit breaker should be turned off, and GOS has to be opened. However to continue power delivery to the affected feeder, Bus coupler has to be closed in order to transfer load on affected feeder to the other transformer which is in service.
This is simulated on below.

1. Initial condition is
   <ul style="list-style-type: disc">
   <li>Both transformer1, transformer2 in service</li>
   <li>Bus coupler (BC) is OFF.</li>
   <li>Transformer1 supplying load on feeder1.</li>
   <li>Transformer2 supplying load on feeder2.</li>
   </ul>

2. Current breaker status table

<table>
<tr>
<th>Circuit breaker </th>
<th>Status</th>
<th> Fixed operation</th>
</tr>

<tr>
<td>CB1</td>
<td> ON </td>
<td>OFF</td>
</tr>

<tr>
<td>CB2 </td>
<td>ON</td>
<td> OFF</td>
</tr>

<tr>
<td>CB3 </td>
<td>ON </td>
<td>OFF</td>
</tr>

<tr>
<td>CB4 </td>
<td>ON</td>
<td> OFF</td>
</tr>

<tr>
<td>CB5</td>
<td> ON</td>
<td> OFF</td>
</tr>

<tr>
<td>CB6</td>
<td> ON </td>
<td>OFF</td>
</tr>

<tr>
<td>CB7 </td>
<td>ON </td>
<td>OFF</td>
</tr>

<tr>
<td>BC</td>
<td> OFF</td>
<td> ON</td>
</tr>
</table>

3. GOS status table

<table>
<tr>
<th>Circuit breaker </th>
<th>Status</th>
<th> Fixed operation</th>
</tr>
<tr>
<td>GOS1 </td>
<td>ON </td>
<td>OFF</td>
</tr>
<tr>
<td>GOS2 </td>
<td>ON </td>
<td>OFF</td>
</tr>

<tr>
<td>GOS3 </td>
<td>ON </td>
<td>OFF</td>
</tr>

<tr>
<td>GOS4 </td>
<td>ON </td>
<td>OFF</td>
</tr>

<tr>
<td>GOS5 </td>
<td>ON </td>
<td>OFF</td>
</tr>

<tr>
<td>GOS6 </td>
<td>ON </td>
<td>OFF</td>
</tr>

</table>

4. Reading of meter

<table>
<tr>
<th>M1 </th>
<th>M2</th>
<th> M3</th>
<th> M4 </th>
<th>M5</th>
</tr>

<td>V=11 kV,<br>
 I=30 A,<br>
P=571.58 kW</td>

<td>V=11 kV,<br>
 I=45 A,<br>
P=857.36  kW</td>

<td>V=33 kV,<br>
 I=25 A,<br>
P=1423.94 kW</td>

<td>V=11 kV,<br>
 I=30 A,<br>
P=571.58 kW</td>

<td>V=11 kV,<br>
 I=45 A,<br>
P=857.36 kW</td>
</table>

<u>Transformer1 is to be taken out for maintenance</u>  
5. Select transformer1, which is to be taken out for maintenance.  
6. Force operation sequence as follows

   <ul style="list-style-type: disc">
<li>BC is changed from OFF to ON.</li>
<li>CB4 is changed from ON to OFF.</li>
<li>CB2 is changed from ON to OFF.</li>
<li>GOS3 is changed from close to open.</li>
<li>Color of GOS3, CB4, CB2 changes to red.</li>
<li>Color of BC changes to green.</li>
</ul>

7. Reading of meter
<table>
<tr>
<th>M1 </th>
<th>M2</th>
<th> M3</th>
<th> M4 </th>
<th>M5</th>
</tr>

<td>V=11 kV,<br>
 I=30 A,<br>
P=571.58 kW</td>

<td>V=11 kV,<br>
 I=45 A,<br>
P=857.36  kW</td>

<td>V=33 kV,<br>
 I=25 A,<br>
P=1423.94 kW</td>

<td>V=0 kV,<br>
 I=0 A,<br>
P=0 kW<br>
(=M1)
</td>

<td>V=11 kV,<br>
 I=75 A,<br>
P=1428.94 kW<br>
(=M2)
</td>
</table>

<u>Transformer1 is to be brought into service</u>  
8. Select Transformer1, which is to be brought back into service.  
9. Force operation sequence as follows

   <ul style="list-style-type: disc">
<li>GOS3 is changed from open to close.</li>
<li>CB4 is changed from OFF to ON.</li>
<li> CB2 is changed from OFF to ON.</li>
<li> BC is changed from OFF to ON.</li>
<li> Display color of all CB's and G.O.S changes accordingly.</li>
</ul>

10. Reading of meter

<table>
<tr>
<th>M1 </th>
<th>M2</th>
<th> M3</th>
<th> M4 </th>
<th>M5</th>
</tr>

<td>V=11 kV,<br>
 I=30 A,<br>
P=571.58 kW</td>

<td>V=11 kV,<br>
 I=45 A,<br>
P=857.36  kW</td>

<td>V=33 kV,<br>
 I=25 A,<br>
P=1423.94 kW</td>

<td>V=11 kV,<br>
 I=30 A,<br>
P=571.58 kW<br>
   <ul style="list-style-type: disc">
<li>M1=M4
</li>
</ul></td>

<td>V=11 kV,<br>
 I=45 A,<br>
P=857.36  kW<br>
   <ul style="list-style-type: disc">
<li>M2=M5
</li>
</ul></td>
</table>

11. Repeat the same step for Transformer2 to be taken out for maintenance.
