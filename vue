



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
