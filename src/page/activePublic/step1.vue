<template>
  <!-- //  TODO:这个页面有一个不足之处，时间选择器组件，表单验证出错，这是element组件的问题，留给大家自己去完善 -->
  <div class="step1">
    <!-- element表单组件 -->
    <el-form :model="ruleForm" class="demo-ruleForm" :rules="rules" ref="ruleForm" label-position="top">
      <!-- 表单项，prop属性表示要进行表单验证，验证规则对应为rules的属性name -->
      <el-form-item label="活动名称" prop="name">
          <el-input v-model="ruleForm.name" size="large"></el-input>
      </el-form-item>
      <el-form-item label="" prop="fenLei">
        <!-- 改装后的表单项，在标签栏添加了一个按钮 -->
        <el-row style="height: 35px;" type="flex" align="middle">
          <el-col :span="3" style="width: 90px;">
            <div class="el-form-item__label" style="padding-bottom: 0;">活动分类</div>

          </el-col>
        </el-row>
      </el-form-item>
    </el-form>
  </div>
</template>
