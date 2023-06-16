'/ms/serverComputingGetdata': {
            target:
              // 'https://smartde.libing-beta.rnd.huawei.com/smartdm/rest/serverComputingGetdata',
              'http://10.235.46.153:8824',
            changeOrigin: true,
            pathRewrite: {
              '^/ms/serverComputingGetdata': '/'
            }
          },
          '/ms': {
            target: 'https://smartde.libing-beta.rnd.huawei.com/smartdm/ms', // ms
            changeOrigin: true,
            pathRewrite: {
              '^/ms': '/'
            }
          },
https://blog.csdn.net/BellaShang/article/details/123236465
this.$refs['title'] && this.$refs['title'][0].$el.scrollIntoView({
            behavior: 'smooth'
          })


// 取消上传动作
        this.$refs['syncContinueUpload'][0].abort(file);
        // 设置 手动取消 上传状态 ，on-before 中使用
        file['dmCancel'] = true;
        return false;
        this.$refs[`uploadAttachmentRef${field.fieldName}`][0].$refs['upload-inner'].handleClick()

https://blog.csdn.net/The_Moon_/article/details/127959648

const dataWatcher = this.$watch('data', (newVal, oldVal) => {
            this.formData = _.cloneDeep(newVal)
            if (dataWatcher) {
                dataWatcher()
            }
        }, { deep: true })


 &:hover {
        .file-item-icon {
          .success-icon {
            display: none;
          }
          .del-icon {
            display: inline-block;
          }
        }
      }

formatCol () {
      this.table.col = this.table.col.map(item => {
          if(item.name === 'changed') {
            item.formatter = (row, column, cellValue) => {
              return (<span>{cellValue === '1' ? '是' : '否'}</span>)
            }
          }
          else if(item.name === 'operate') {
            item.formatter = (row, column, cellValue) => {
              return (<el-button type="text" disabled={row.changed === '1'}>替换</el-button>)
            }
          }
          return item
      })
    }

https://blog.csdn.net/ZYS10000/article/details/123243486


https://blog.csdn.net/qq_46149597/article/details/127694582
https://blog.csdn.net/ZMJ_QQ/article/details/122327481
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
