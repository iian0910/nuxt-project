<template>
  <div>
    <el-container>
      <el-main>
        <el-row>
          <el-col :span="24"><div class="grid-content bg-purple-dark"></div></el-col>
        </el-row>
        <el-row :gutter="30">
          <!--
            xs    : < 768px
            sm    : ≥ 768px   (768px ~ 991px)
            md    : ≥ 992px   (992px ~ 1199px)
            lg    : ≥ 1200px  (1200px ~ 1919px)
            xl    : ≥ 1920px
          -->
          <el-col
            :xs="24"
            :sm="6"
            :md="4"
            :lg="3"
            :xl="1"
          ><div class="grid-content bg-purple"></div></el-col>
          <el-col :xs="24" :sm="6" :md="8" :lg="9" :xl="11"><div class="grid-content bg-purple-light"></div></el-col>
          <el-col :xs="24" :sm="6" :md="8" :lg="9" :xl="11"><div class="grid-content bg-purple"></div></el-col>
          <el-col :xs="24" :sm="6" :md="4" :lg="3" :xl="1"><div class="grid-content bg-purple-light"></div></el-col>
        </el-row>
      </el-main>
    </el-container>
  </div>
</template>
<script>
export default {

}
</script>
<style lang="scss">
.el-row {
  margin-bottom: 20px;
  &:last-child {
    margin-bottom: 0;
  }
}
.el-col {
  border-radius: 4px;
}
.bg-purple-dark {
  background: #99a9bf;
}
.bg-purple {
  background: #d3dce6;
}
.bg-purple-light {
  background: #e5e9f2;
}
.grid-content {
  border-radius: 4px;
  min-height: 36px;
}
.row-bg {
  padding: 10px 0;
  background-color: #f9fafc;
}
</style>
