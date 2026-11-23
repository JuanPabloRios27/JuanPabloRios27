<!--options-->
<table>
  <tr>
    <td align="center" nowrap="nowrap">Option</i></td><td align="center" nowrap="nowrap">Description</td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_isocalendar</code></h4></td>
    <td rowspan="2"><p>Enable isocalendar plugin</p>
<img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>boolean</code>
<br>
<b>default:</b> no<br></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_isocalendar_duration</code></h4></td>
    <td rowspan="2"><p>Time range</p>
<ul>
<li><code>half-year</code>: 180 days</li>
<li><code>full-year</code>: 1 year</li>
</ul>
<img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>string</code>
<br>
<b>default:</b> half-year<br>
<b>allowed values:</b><ul><li>half-year</li><li>full-year</li></ul></td>
  </tr>
</table>
<!--/options-->

## ℹ️ Examples workflows

<!--examples-->
```yaml
name: Half-year calendar
uses: lowlighter/JuanPabloRios27@latest
with:
  filename: metrics.plugin.isocalendar.svg
  token: ${{ secrets.METRICS_TOKEN }}
  base: ""
  plugin_isocalendar: yes

```
```yaml
name: Full-year calendar
uses: lowlighter/JuanPabloRios27@latest
with:
  filename: metrics.plugin.isocalendar.fullyear.svg
  token: ${{ secrets.METRICS_TOKEN }}
  base: ""
  plugin_isocalendar: yes
  plugin_isocalendar_duration: full-year

```
<!--/examples-->
