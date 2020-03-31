

http://172.20.95.130:8086/
线上环境已经部署好，用户名密码都是hiuser

172.20.95.130，俊刚，这个服务器，用    root  密  smartdot。
然后在/root/temp目录下，我把项目打包了，idea下可用



资料
https://helicalinsight.github.io/helicalinsight/#/create-efw-report << Creating Reports and Dashboards >>

http://www.helicalinsight.com/technical-guide/efw-for-report-creation/

http://www.helicalinsight.com/helical-insight-ce/how-to-create-dashboard-in-helical-insight-ce/

https://ee3q7p.axshare.com 原型

SFTP
172.20.95.130
root / smartdot
/report/hi-repository/Sample Reports
http://172.20.95.130:8086/



1. 怎么添加面板？
2. 面板上的如何动态添加视图？
		let components = [pieChart];
		dashboard.init(components);

3. 视图是否可显示浮窗？
4. 如何控制视图位置、大小？
5. 如何保存视图状态？

栅格数 12

***.html = dashboard

<div class="chart c3" id="chart_2">
    <svg>
        图表
    </svg>
</div>


Set - dashboard.setVariable('gender', 'male'); 
Get - var gender = dashboard.getVariable('gender');

.efw > .html > .efwvf > .efwd 


图表库 c3
var chart = c3.generate({
								bindto: '#chart_2',
								data: {
									columns: array1,
									type: 'pie'
								},
								legend: {
									show: true
								},
								tooltip: {
								  show: true
								}
							});	
