## 计费规则<br>
<table>
     <tr align="center">
        <th width="300">产品名称</th>
        <th width="300">费项</th>
     </tr>
      <tr>
         <td rowspan="3" align="center">流数据总线</td>
         <td>读写次数</td>
      </tr>
      <tr>
         <td>吞吐量</td>
      </tr>
      <tr>
         <td>存储时间</td>
      </tr>
</table>

<br>

**名词解释**<br>
读写次数: <br>
数据流的计费单元，以64KB有效载荷计算，以每百万记录收费，例如，5KB消息按照一个记录收费，90KB消息按照两个记录收费<br>
<br>
吞吐量:<br>
每个单位吞吐量最大支持1MB/s写入,2MB/s读取能力，或者1000条消息/s写入，2000条消息读取的消息读写处理能力\<br>
<br>
存储时间:<br>
数据在流数据总线的存储时间, 默认为1天, 最大存储7天<br>
<br>

## 欠费规则

* 当您的流数据总线服务在扣取前一天的账单费用失败时，会视为处于欠费状态。<br>
* 欠费后流数据总线服务将会立刻自动停止，且停止扣费。<br>
* 若您在欠费后15 天内充值补足欠款后，服务会自动开启，可以继续使用；若欠费超过 15 天没有补足欠款，将视为您主动放弃流数据总线服务, 服务停止后，未处理的消息数据将自动释放，被释放的数据不可恢复。<br>
