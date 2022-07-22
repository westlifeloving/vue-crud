<template>
  <el-container style="height: 100%; border: 1px solid #eee">
    <el-aside width="200px" style="background-color: rgb(238, 241, 246)">
      <el-menu
        :default-openeds="[]"
        background-color="#545c64"
        text-color="#fff"
      >
        <el-submenu index="1">
          <template slot="title"><i></i>域名管理</template>
          <el-menu-item index="1-1">服务概览</el-menu-item>
          <el-menu-item index="1-2">域名列表</el-menu-item>
          <el-menu-item index="1-3">流量记录</el-menu-item>
          <el-menu-item index="1-4">通用设置</el-menu-item>
        </el-submenu>
        <el-submenu index="2">
          <template slot="title"><i></i>抗D保</template>
          <el-menu-item index="2-1">概览</el-menu-item>
          <el-menu-item index="2-2">报表</el-menu-item>
          <el-menu-item index="2-3">功能管理</el-menu-item>
          <el-menu-item index="2-4">智慧引擎</el-menu-item>
          <el-menu-item index="2-5">DDos告警</el-menu-item>
          <el-menu-item index="2-6">日志下载</el-menu-item>
        </el-submenu>
        <el-submenu index="3">
          <template slot="title"><i></i>创宇盾(WAF)</template>
          <el-menu-item index="3-1">概览</el-menu-item>
          <el-menu-item index="3-2">报表</el-menu-item>
          <el-menu-item index="3-3">功能管理</el-menu-item>
          <el-menu-item index="3-4">日志下载</el-menu-item>
        </el-submenu>
        <el-submenu index="4">
          <template slot="title"><i></i>加速乐(SCDN)</template>
          <el-menu-item index="4-1">概览</el-menu-item>
          <el-menu-item index="4-2">报表</el-menu-item>
          <el-menu-item index="4-3">缓存刷新</el-menu-item>
          <el-menu-item index="4-4">功能管理</el-menu-item>
          <el-menu-item index="4-5">日志下载</el-menu-item>
        </el-submenu>
        <el-submenu index="5">
          <template slot="title"><i></i>应用保</template>
          <el-menu-item index="5-1">功能设置</el-menu-item>
          <el-menu-item index="5-2">报表</el-menu-item>
        </el-submenu>
        <el-submenu index="6">
          <template slot="title"><i></i>数据盾</template>
          <el-menu-item index="6-1">功能设置</el-menu-item>
          <el-menu-item index="6-2">报表</el-menu-item>
        </el-submenu>
        <el-submenu index="7">
          <template slot="title"><i></i>净网盾</template>
          <el-menu-item index="7-1">功能设置</el-menu-item>
          <el-menu-item index="7-2">报表</el-menu-item>
        </el-submenu>
        <el-submenu index="8">
          <template slot="title"><i></i>隐私盾</template>
          <el-menu-item index="8-1">功能设置</el-menu-item>
          <el-menu-item index="8-2">报表</el-menu-item>
        </el-submenu>
        <el-submenu index="9">
          <template slot="title"><i></i>SSL安全网关</template>
          <el-menu-item index="9-1">功能设置</el-menu-item>
        </el-submenu>
        <el-submenu index="10">
          <template slot="title"><i></i>HTTPDNS</template>
          <el-menu-item index="10-1">功能设置</el-menu-item>
          <el-menu-item index="10-2">报表</el-menu-item>
        </el-submenu>
        <el-submenu index="11">
          <template slot="title"><i></i>实时防御动态图</template>
          <el-menu-item index="11-1">功能设置</el-menu-item>
        </el-submenu>
        <el-submenu index="12">
          <template slot="title"><i></i>威胁情报</template>
          <el-menu-item index="12-1">威胁情报查询</el-menu-item>
          <el-menu-item index="12-2">协同防御查询</el-menu-item>
        </el-submenu>
        <el-submenu index="13">
          <template slot="title"><i></i>告警中心</template>
          <el-menu-item index="13-1">告警总览</el-menu-item>
          <el-menu-item index="13-2">告警设置</el-menu-item>
        </el-submenu>
        <el-submenu index="14">
          <template slot="title"><i></i>增值服务</template>
          <el-menu-item index="14-1">高级设置</el-menu-item>
          <el-menu-item index="14-2">增值模块</el-menu-item>
          <el-menu-item index="14-3">API管理</el-menu-item>
        </el-submenu>
        <el-submenu index="15">
          <template slot="title"><i></i>证书购买</template>
          <el-menu-item index="15-1">自助购买</el-menu-item>
          <el-menu-item index="15-2">订单管理</el-menu-item>
        </el-submenu>
        <el-submenu index="16">
          <template slot="title"><i></i>系统管理</template>
          <el-menu-item index="16-1">日志下载</el-menu-item>
          <el-menu-item index="16-2">操作日志</el-menu-item>
          <el-menu-item index="16-3">子账户</el-menu-item>
          <el-menu-item index="16-4">角色权限</el-menu-item>
        </el-submenu>
      </el-menu>
    </el-aside>

    <el-container>
      <el-header>
        <el-menu
          class="el-menu-demo"
          mode="horizontal"
          background-color="#545c64"
          text-color="#fff"
          active-text-color="#ffd04b"
        >
          <el-menu-item index="1">控制台首页</el-menu-item>
          <el-submenu index="2">
            <template slot="title">产品控制面板</template>
            <el-submenu index="2-1">
              <template slot="title">技术安全</template>
              <el-menu-item index="2-1-1">抗D保</el-menu-item>
              <el-menu-item index="2-1-2">创宇盾</el-menu-item>
              <el-menu-item index="2-1-3">加速乐</el-menu-item>
              <el-menu-item index="2-1-4">创宇监控</el-menu-item>
              <el-menu-item index="2-1-5">漏洞扫描</el-menu-item>
            </el-submenu>
            <el-submenu index="2-2">
              <template slot="title">业务安全</template>
              <el-menu-item index="2-2-1">护架卫士</el-menu-item>
              <el-menu-item index="2-2-2">羊毛盾</el-menu-item>
              <el-menu-item index="2-2-3">净网盾</el-menu-item>
              <el-menu-item index="2-2-4">数据盾</el-menu-item>
              <el-menu-item index="2-2-5">流量反欺诈</el-menu-item>
              <el-menu-item index="2-2-6">金融反欺诈</el-menu-item>
              <el-menu-item index="2-2-7">ScanA网站内容安全</el-menu-item>
              <el-menu-item index="2-2-8">云监测</el-menu-item>
            </el-submenu>
            <el-submenu index="2-3">
              <template slot="title">商业安全</template>
              <el-menu-item index="2-3-1">SSL证书</el-menu-item>
            </el-submenu>
            <el-submenu index="2-4">
              <template slot="title">安全服务</template>
              <el-menu-item index="2-4-1">渗透测试</el-menu-item>
              <el-menu-item index="2-4-2">代码审计</el-menu-item>
            </el-submenu>
          </el-submenu>
          <el-submenu index="3">
            <template slot="title">消息</template>
            <el-menu-item index="3-1">站内消息</el-menu-item>
          </el-submenu>
          <el-submenu index="4">
            <template slot="title">费用</template>
            <el-menu-item index="4-1">账户余额</el-menu-item>
            <el-menu-item index="4-2">我的订单</el-menu-item>
            <el-menu-item index="4-3">收支明细</el-menu-item>
            <el-menu-item index="4-4">优惠券</el-menu-item>
            <el-menu-item index="4-5">发票管理</el-menu-item>
          </el-submenu>
          <el-menu-item index="5">帮助</el-menu-item>
          <el-submenu class="userinfor" index="6">
            <template slot="title">admin</template>
            <el-menu-item index="6-1">基本信息</el-menu-item>
            <el-menu-item index="6-2">地址管理</el-menu-item>
            <el-menu-item index="6-3">重制密码</el-menu-item>
            <el-menu-item index="6-4">安全退出</el-menu-item>
          </el-submenu>
        </el-menu>
      </el-header>

      <el-main>
        <el-breadcrumb style="margin: 0 0 30px" separator="/">
          <el-breadcrumb-item :to="{ path: '/' }">创宇盾</el-breadcrumb-item>
          <el-breadcrumb-item><a href="/">防御设置</a></el-breadcrumb-item>
          <el-breadcrumb-item>精准访问控制</el-breadcrumb-item>
        </el-breadcrumb>
        <el-row style="margin: 20px 0">
          <el-page-header title="" back="" content="精准访问控制策略"
            >精准访问控制策略</el-page-header
          >
        </el-row>
        <el-row>
          <div>
            <el-button type="primary" @click="goPushColumn('add')">添加策略</el-button>
            <span style="font-size: 10px; color: grey; margin-left: 15px"
              >最多可添加20条策略。</span
            >
            <push-dialog
              :add-strategy="addStrategy"
              @pushDialogHide="hideDialog"
              :open.sync="pushDialogOpen"
              :choose.sync="isEdit"
            >
            </push-dialog>
          </div>
        </el-row>
        <el-table
          ref="multipleTable"
          :data="tableData"
          tooltip-effect="dark"
          :header-cell-style="{ background: 'rgb(64,158,255,0.1)' }"
          style="
            margin: 15px 0;
            width: 100%;
            border: 1px solid #dcdfe6;
            border-radius: 4px;
          "
          @selection-change="handleSelectionChange"
        >
          <el-table-column type="selection" width="55"> </el-table-column>
          <el-table-column prop="name" label="策略名称" width="130">
          </el-table-column>
          <el-table-column prop="condition" label="匹配条件" width="120">
          </el-table-column>
          <el-table-column prop="action" label="匹配动作"> </el-table-column>
          <el-table-column prop="port" label="生效端口"> </el-table-column>
          <el-table-column prop="priority" label="优先级"> </el-table-column>
          <el-table-column prop="switch" label="策略开关">
            <el-switch
              v-model="switchvalue"
              active-color="#409EFF"
              inactive-color="#C1D0DB"
            >
            </el-switch>
          </el-table-column>
          <el-table-column prop="operation" label="操作">
            <template slot-scope="scope">
              <el-button @click="goPushColumn('edit')" type="text" size="small"
                >修改</el-button
              >
              <el-button
                @click.native.prevent="deleteRow(scope.$index, tableData)"
                type="text"
                size="small"
                >删除</el-button
              >
              <push-dialog
                @pushDialogHide="hideDialog"
                :open.sync="pushDialogOpen"
              >
              </push-dialog>
            </template>
          </el-table-column>
        </el-table>
        <el-row>
          <el-button
            @click="delAll()"
            style="border: none; color: #c0c4cc; font-size: 12px"
            type="text"
            size="small"
            >批量删除</el-button
          >
        </el-row>
      </el-main>
    </el-container>
  </el-container>
</template>

<script>
import PushDialog from "@/components/pushDialog.vue";
export default {
  name: "vueStrategy",
  components: { PushDialog },
  data() {
    return {
      pushDialogOpen: false,
      tableData: [
        {
          id: "1",
          name: "示例规则_账号爆破防护",
          condition: "URI 包含 /login  HTTP-Method 等于 POST  Referer 不存在",
          action: "阻断",
          port: "全部",
          priority: "1",
        },
        {
          id: "2",
          name: "示例规则_API防护",
          condition: "URI 包含 /api/  User-Agent 不等于 specialUA",
          action: "阻断",
          port: "全部",
          priority: "2",
        },
        {
          id: "3",
          name: "示例规则_网络爬虫放行",
          condition: "User-Agent 包含 spider",
          action: "放行",
          port: "全部", 
          priority: "3",
        },
      ],
      multipleSelection: [],
      switchvalue: false,
      isEdit: true,
    };
  },

  methods: {
    addStrategy(newStrategy){
      this.tableData = [...this.tableData, newStrategy];
      console.log(this.tableData)
    },
    goPushColumn(type) {
      this.pushDialogOpen = true;
      if(type=='add'){
        this.isEdit = true;
      }
      else if(type=='edit'){
        this.isEdit = false;
      }
    },

    hideDialog() {
      this.pushDialogOpen = false;
    },
    toggleSelection(rows) {
      if (rows) {
        rows.forEach((row) => {
          this.$refs.multipleTable.toggleRowSelection(row);
        });
      } else {
        this.$refs.multipleTable.clearSelection();
      }
    },
    handleSelectionChange(val) {
      this.multipleSelection = val;
    },
    handleEdit(index, row) {
      console.log(index, row);
    },
    deleteRow(index, rows) {
      this.$confirm("确定删除该策略吗", {
        confirmButtonText: "确定",
        cancelButtonText: "取消",
        type: "success",
        callback: (action) => {
          if (action === "confirm") {
            rows.splice(index, 1);
          }
        },
      });
    },
    openDialog() {
      this.dialogFormVisible = true;
    },
    delAll() {
      var d = this.tableData;
      this.$refs.multipleTable.selection.forEach((Ele, index) => {
        for (var i = 0; i < d.length; i++) {
          var t = d[i].id;
          if (t == Ele.id) {
            d.splice(i, 1);
          }
        }
        console.log(index);
      });
    },
  },
};
</script>

<style>
.el-header {
  color: #333;
  line-height: 60px;
}

.el-aside {
  color: #333;
}

.note {
  color: rgb(255, 196, 0);
  font-size: 10px;
  margin: 0 0 0 10px;
}

.el-dialog {
  margin-left: 40vh;
}

.el-divider--horizontal {
  margin: 10px 0 15px 0 !important;
}

.el-dialog__body {
  padding: 0px 20px !important;
}

.el-form-item__label {
  width: 80px !important;
}

.el-form-item__content {
  margin-left: 100px !important;
}

.addname {
  width: 40% !important;
}

.el-page-header__left .el-icon-back {
  font-size: 0px !important;
  margin-right: 0px !important;
}

[class*=" el-icon-"],
[class^="el-icon-"] {
  font-family: Arial, Helvetica, sans-serif !important;
}

.el-page-header__left {
  margin-left: -20px !important;
}

.el-page-header__left::after {
  background-color: #0080ff !important;
  width: 2px !important;
}
/* .el-menu--horizontal>.el-submenu {
  margin-right: 30px !important;
} */
</style>
