
<template>
  <div class="page-container">
    <div class="page-content">
    <el-pagination
      @size-change="handleSizeChange"
      @current-change="handleCurrentChange"
      :current-page="currentPage"
      :page-sizes="[10, 20, 50, 100]"
      :page-size="pageSize"
      layout="total, sizes, prev, pager, next, jumper"
      :total="total"
    ></el-pagination>
    </div>
  </div>
</template>
<script>
// <pagination-self :total="table.total" @paginationListen="paginationListen" ></pagination-self>

// 详情监听
// paginationListen ({currentPage, pageSize}) {
//   this.table.currentPage = currentPage
//   this.table.pageSize = pageSize
//   this.getTable()
// },

export default {
  props: {
    total: {
      type: Number,
      default: 0
    },
    pCurrentPage: {
      type: Number,
      default: 1
    },
    pPageSize: {
      type: Number,
      default: 10
    }
  },
  data () {
    return {
      currentPage: 1, // 当前页
      pageSize: 10   // 每页条数
    }
  },
  watch: {
    pCurrentPage (newVal, oldVal) {
      this.currentPage = newVal
    },
    pPageSize (newVal, oldVal) {
      this.pageSize = newVal
    }
  },
  methods: {
    // 条数切换
    handleSizeChange (val) {
      this.currentPage = 1
      this.pageSize = val
      this.$emit('paginationListen', {currentPage: this.currentPage, pageSize: this.pageSize})
    },
    // 页码切换
    handleCurrentChange (val) {
      this.currentPage = val
      this.$emit('paginationListen', {currentPage: this.currentPage, pageSize: this.pageSize})
    }
  }
}
</script>










        let total = Array.from(new Set([...table2Arr]))
localStorage、vuex全局变量以路由标识依据
一个整个流程使用一个路由
$emit.off
https://blog.csdn.net/weixin_42927679/article/details/128630362
https://zhidao.baidu.com/question/1759992812723929508.html
https://blog.csdn.net/qq_25252769/article/details/120280815
https://blog.csdn.net/zhao949895887/article/details/121220299
https://googlechrome.github.io/devtools-samples/jank/

import FileSaver from 'file-saver'
import XLSX from 'xlsx'

exportTableCheckData (tableId, fileName) {
      try {
        let wb = XLSX.utils.table_to_book(document.querySelector('#' + tableId)); // el-table id
        let wbout = XLSX.write(wb, { bookType: 'xlsx', bookSST: true, type: 'array' });
        FileSaver.saveAs(new Blob([wbout], { type: 'application/octet-stream' }), fileName + Date.parse(new Date()) + '.xlsx');
        return wbout
      } catch (e) {
        if (typeof console !== 'undefined')
          console.log(e, wbout)
      }
    }


myChart.getZr().on("click", function (params) {
              const pointInPixel = [params.offsetX, params.offsetY];
              if (myChart.containPixel("grid", pointInPixel)) {
                let xIndex;
                if (parameterMap.conditionType == "客户") {
                  xIndex = myChart.convertFromPixel({ seriesIndex: 0 }, pointInPixel)[0];
                } else {
                  xIndex = myChart.convertFromPixel({ seriesIndex: 0 }, pointInPixel)[1];
                }
                parameterMap['paramName'] = xaxisDatas[xIndex];
                _that.getMonthGroupInventoryDashboard(parameterMap, "childEcharts")
              }
            })
