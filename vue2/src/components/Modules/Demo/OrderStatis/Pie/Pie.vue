<template>
    <section class="chart">
        <el-row>
            <el-col :span='24'>
                <el-button
                    type="primary"
                    @click='onUpdateTitle'>更新标题</el-button>
                <el-button
                    type="primary"
                    @click='onUpdateSubtext'>更新标题下面的描述</el-button>
                <el-button
                    type="primary"
                    @click='onUpdateHoverTitle'>更新鼠标放上去的标题</el-button>
                <el-button
                    type="primary"
                    @click='onUpdateValueList'>更新数据值</el-button>
                <el-button
                    type="primary"
                    @click='onUpdateTextList'>更新数据字段名</el-button>
            </el-col>

            <el-col :span="24">
                <statis
                	:id='echarts_data.id'
                	:title='echarts_data.title'
                	:subtext='echarts_data.subtext'
                	:hoverTitle='echarts_data.hover_title'
                	:dataList='echarts_data.data_list'></statis>
            </el-col>
        </el-row>
    </section>
</template>
<script>
    import PieJs from './Pie.js';
    module.exports=PieJs;
</script>
<style scoped>
    
</style>
