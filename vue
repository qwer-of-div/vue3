



https://blog.csdn.net/ag_wenbi/article/details/122208018
this.$refs['title'] && this.$refs['title'][0].$el.scroll({
            behavior: 'smooth'
          })
    this.$refs.piNames1.$el.querySelector('input').focus()

  scroll-behavior: smooth;


ishas ? this.editFormData = datas : this.noData = '当前没有配置表单!'

onInput :debounce(function() {
      this.getba()
    }, 500),

const routeUrl = this.$router.resolve({
              path: '/deliver_project_process/detail',
              query: { jiraNum: data }
            })
            window.open(routeUrl.href, '_blank')



pickerOptions: {},  // 开始日期限制
    // 年份禁用
    handleDisabledDate (key = "pickerOptions", date1 = new Date('2019-01-01')) {
      this.init[key] = {}
      if (key === "pickerOptions") {
        this.init[key].disabledDate = (date) => {
          const zero = date1.setHours(0, 0, 0, 0);
          // disabledDate 为true表示不可选,false表示可选
          if (date.getTime() < zero) return true;
          return false;
        }
      } else {
        this.init[key].disabledDate = (date) => {
          // 传入时间
          const zero = date1.setHours(0, 0, 0, 0);
          const endDate = this.$moment(date1).add(1, 'y')._d;
          const endDate1 = endDate.setHours(0, 0, 0, 0);
          // disabledDate 为true表示不可选, false表示可选
          if (date.getTime() < zero || date.getTime() > endDate1) return true;
          return false;
        }
      }
    },


height 100% 等于 内容区的高度 boxing-sizing: 

https://blog.csdn.net/weixin_43924896/article/details/122945886


exportTableCheckData (tableId, fileName) {
      try {
        let wb = XLSX.utils.table_to_book(document.querySelector('#' + tableId));
        let wbout = XLSX.write(wb, { bookType: 'xlsx', bookSST: true, type: 'array' });
        FileSaver.saveAs(new Blob([wbout], { type: 'application/octet-stream' }), fileName + Date.parse(new Date()) + '.xlsx');
        return wbout
      } catch (e) {
        if (typeof console !== 'undefined')
          console.log(e, wbout)
      }
    },
https://blog.csdn.net/yhj198927/article/details/124266388
this.$refs.ruleForm.validateField(['faultyProductVersion', 'prooductVersion'])

export const searchFiled = [
    {label: '分支名', name: 'branchName', type:'input',  placeholder: '', multCtrol: ['exception'], ctrol: [
        {value: ['主干'], ctrolList: [
            {ctrolName: 'planRecycteDate', ctrolValue: 'master', ctrolFiled: {isHide: true}}
        ]}
    ]},
    {label: '对应C版本', name: 'libingVersion', options: [], loading: false, type: 'selectSearch'},
    {label: '是否例外申请', name: 'exception', type:'select', options: options.yesNo, required: true,
    multCtrolTo: [
        {
            branchName: ['1'],
            submit: ['转交'],
            ctrolFiled: {isHide: true},
        }
    ]}
]

handleCtrol (value, filed) {
            // 多控
            if(filed.ctrol) {
                // 多控数组循环
                for(const ct of filed.ctrol) {
                    // filedList循环
                    for(const fiLi of this.filedList) {
                        // 找到被控制的值
                        for(const ctrolItem of ct.ctrolList) {
                            if(fiLi.name === ctrolItem.ctrolName) {
                                // 值等于多少的时候触发
                                if(ct.value === value) {
                                    // 赋值
                                    if(ctrolItem.ctrolValue !== null) {
                                        this.form[ctrolItem.ctrolName] = ctrolItem.ctrolValue
                                    }
                                    if(ctrolItem.ctrolFiled) {
                                        for(let key in ctrolItem.ctrolFiled) {
                                            fiLi[key] = ctrolItem.ctrolFiled[key]
                                        }
                                    }
                                } else {
                                    // 找到初始的item 恢复默认值
                                    this.form[ctrolItem.ctrolName] = this.formClone[ctrolItem.ctrolName]
                                    const itemCopy = this.filedListClone.find( el => el.name === ctrolItem.ctrolName)
                                    for(let key in itemCopy) {
                                        fiLi[key] = itemCopy[key]
                                    }
                                }
                                // 已找到控制的filed 退出
                                break
                            }
                        }
                    }
                }
            }
        }




                      https://blog.csdn.net/qq_43127921/article/details/101291107
https://www.cnblogs.com/bala/p/16378285.html
https://blog.csdn.net/SongZhengxing_/article/details/125480697
https://blog.csdn.net/qq_44844751/article/details/124006018
https://blog.csdn.net/weixin_43843572/article/details/124980771
所有需要登录的都为子路由

https://blog.csdn.net/weixin_46801545/article/details/126041079



                      




