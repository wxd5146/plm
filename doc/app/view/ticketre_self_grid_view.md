# 工单(ticketre_self_grid_view)  <!-- {docsify-ignore-all} -->




<el-skeleton style="width:60%">
	<template #template>
		<div style="padding-bottom: 5px;">
			<div style="height:40px;display: flex;align-items: center;justify-content: space-between;">
				<el-tooltip content="页面标题">
					<el-skeleton-item variant="text" style="height:40px;"></el-skeleton-item>
				</el-tooltip>
				<el-tooltip content="搜索栏">
				    <el-skeleton-item variant="text" style="margin-left: 10px;height:40px;width:300px;"></el-skeleton-item>
				</el-tooltip>
				<el-skeleton style="width:250px;">
					<template #template>
						<el-tooltip content="工具栏">
							<div style="display: flex;align-items: center;justify-content:end">
								<el-skeleton-item variant="text" style="margin-left: 10px;height:40px;width:80px"></el-skeleton-item>
								<el-skeleton-item variant="text" style="margin-left: 10px;height:40px;width:80px"></el-skeleton-item>
								<el-skeleton-item variant="text" style="margin-left: 10px;height:40px;width:80px"></el-skeleton-item>
							</div>
						</el-tooltip>
					</template>
				</el-skeleton>
			</div>
		</div>
		<el-tooltip content="数据表格">
			<el-skeleton-item variant="p" style="height:300px"></el-skeleton-item>
		</el-tooltip>
	</template>
</el-skeleton>


## 控件
  * CAPTIONBAR(captionbar)
  * 工具栏(toolbar)
  * 搜索栏(searchbar)
  * 数据表格(grid)


### 关联界面行为
  * [工单(TICKET)](module/ProdMgmt/Ticket) : [取消关联](module/ProdMgmt/Ticket#界面行为)
  * [工单(TICKET)](module/ProdMgmt/Ticket) : [添加工单（其他实体关联）](module/ProdMgmt/Ticket#界面行为)

### 关联视图
  * [工单(ticketcreate_re_ticket_view)](app/view/ticketcreate_re_ticket_view)
  * [工单(ticketmain_view)](app/view/ticketmain_view)

<script>
 const { createApp } = Vue
  createApp({
    data() {
      return {
        message: '!'
      }
    }
  }).use(ElementPlus).mount('#app')
</script>