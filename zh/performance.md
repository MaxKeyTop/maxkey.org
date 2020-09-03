---
layout: zh/default
---
<h2>性能测试报告</h2>


环境配置 centos7.6  16核 16G

<table border="0" class="table table-striped table-bordered ">
	<thead>
		<th></th><th>600并发/600s</th><th>1200并发/600s</th><th>1600并发/600s</th><th>2400并发/600s</th>
	</thead>
	<tbody>
		<tr>
			<td>响应时长(90%)</td>
			<td>587ms</td>
			<td>924ms</td>
      <td>2695ms</td>
      <td>11m</td>
		</tr>
    <tr>
			<td>总请求量</td>
			<td>1786618</td>
			<td>1659861</td>
      <td>1217766</td>
      <td>1217766</td>
		</tr>
    <tr>
			<td>通过率</td>
			<td>100%</td>
			<td>100%</td>
      <td>100%</td>
      <td>100%</td>
		</tr>
</table>


