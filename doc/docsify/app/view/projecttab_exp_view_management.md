# 项目管理(projecttab_exp_view_management)  <!-- {docsify-ignore-all} -->




<el-skeleton style="width:60%">
	<template #template>
		<div style="padding-bottom: 5px;">
			<div style="height:40px;display: flex;align-items: center;justify-content: space-between;">
				<el-skeleton style="width:250px;">
					<template #template>
						<el-tooltip content="分页栏">
							<div style="display: flex;align-items: center;justify-content:end">
								<el-skeleton-item variant="text" style="height:40px;width:80px"></el-skeleton-item>
								<el-skeleton-item variant="text" style="margin-left: 10px;height:40px;width:80px"></el-skeleton-item>
								<el-skeleton-item variant="text" style="margin-left: 10px;height:40px;width:80px"></el-skeleton-item>
							</div>
						</el-tooltip>
					</template>
				</el-skeleton>
			</div>
		</div>
		<el-tooltip content="导航区占位">
			<el-skeleton-item variant="p" style="height:300px"></el-skeleton-item>
		</el-tooltip>
	</template>
</el-skeleton>


## 控件
  * 分页导航面板(tabexppanel)
  * CAPTIONBAR(captionbar)


### 关联视图
  * [项目管理(projectgrid_view_management_deleted)](app/view/projectgrid_view_management_deleted)
  * [项目管理(projectgrid_view_management_archived)](app/view/projectgrid_view_management_archived)
  * [项目管理(projectgrid_view_management_in_progress)](app/view/projectgrid_view_management_in_progress)

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