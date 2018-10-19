vue中的锚链接跳转问题

在router.js中 
```
//创建 router 实例
const router = new VueRouter({
　　　        routes,
　　　　　　mode: ‘history‘,
　　　　　　scrollBehavior(to, from, savedPosition) {
　　　　　　　　if (to.hash) {
　　　　　　　　　　return {
　　　　　　　　　　　　selector: to.hash
　　　　　　　　　　}
　　　　　　　　}
　　　　　　}
})
export default router;
```

在vue中  点击跳转的位置 使用<a>链接包起来
```
<div>
    <a href="#populationInformation">人口画像</a>
</div>
<div>
    <a href="#peopleCounting">人流统计</a>
</div>
<div>
    <a href="#trafficAnalysis">交通分析</a>
</div>
```

在需要跳转到的位置
```
<div id=‘populationInformation ‘> 人口画像跳转到此</div>
<div id=‘peopleCounting‘> 人流统计跳转到此 </div>
<div id=‘trafficAnalysis ‘>交通分析跳转到此 </div>
```
