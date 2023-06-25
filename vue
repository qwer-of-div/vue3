



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



                      绩效事实
【工作产出】主要包含SmartDM新需求的开发、旧系统项目重构、代码重复率整改以及bug处理任务，独立开发新版【版本管理状态报告】需求，以提供给客户更好的视觉体验，累计上库代码行数1W+，且无线上问题。
【效率提升】学习组合式api的思想、使用async/await新方法优化项目代码，是项目代码观感更友好。发现项目依赖包的高危漏洞并100%解决了它们，修改项目串行代码为并行代码提升页面响应速度。
在完成日常工作的同时，优化前端感官效果，提高用户使用体验，减少代码冗余等
【团队贡献】积极配合同事工作，高效完成工作。对当前项目提出自己的观点与同事进行分析讨论，改进和优化项目。

【效率提升】主动学习前端新知识和新技术，跟上技术的更新换代，保持项目的活力。处理老项目迁移至新项目任务，使用新的架构，采用新的标准，做到页面风格统一规范。
在完成日常工作的同时，提升项目的响应速度，提高用户使用体验，前端感官效果，减少代码冗余等

【主动承担】主动学习前端新知识和新技术，并把新知识和新技术所使用的思想应用于当前项目，对当前项目提出自己的观点与同事进行分析讨论，改进和优化项目。
【能力提升】学习vue3的组合api思想、新版路由管理、状态管理、reactive变量、globalProperties全局变量、keep-alive缓存不活动的组件，为日后更好的工作做准备。

【工作产出】近1年以来，开发累计上库代码5W+，独立负责并完成多个功能模块重构及10+新需求的开发并高质量交付，需求100%及时交付，零客户投诉，需求开发全过程记录并100%可回溯；
对用户的需求积极响应，及时沟通，快速解决，用户满意度极高。
【效率提升】完成SmartDM项目多个功能模块重构，性能提高80%以上，极大的提高了用户体验感，代码冗余率降低90%以上，100%解决了旧代码的维护困难、数据集成传递丢失率高的窘境。
【团队贡献】维护代码包6个，完成代码检视100余次、并提出整改建议或措施150+。





华为业务群个人绩效承诺书
1、拷贝老项目代码到新项目，替代原有依赖，使用当前项目依赖
2、当原有项目设计参数条时，需要重新参数条信息，若原有页面较简单且包含参数条可重构页面
3、迁移完后对比迁移前后的功能点是否一致，测试一致后方可部署生产环境

1、对照原始页面使用ElementUI进行重新布局
2、重新书写页面逻辑，使用新项目封装的方法代替原始方法

1、严格按照开发文档进行开发，不可遗漏任何功能点，如果对需求理解不清晰或者有疑问，及时与责任人沟通解决。
2、根据业务需求撰写页面逻辑
3、与后端联调，拿到数据结合前端页面逻辑完成项目

1、学习vue.js 3.0新的语法，使用函数式编程
2、学习vue.js 3.0新的全局变量定义方式
3、学习不同于webpack的新构建工具vite
4、使用typescript方式书写代码

在工作中以团队利益为主，但也不会忽略个人感受，换位思考别人的个人感受，工作中诚实守信，积极汇报自己工作中的失误和不足

积极争取加分，快速且高效的完成客户要求。

尽量避免减分，如有减分以公司减分标准执行




人员盘点模板
熟悉DIV+CSS布局的HTML代码编写，熟练手写符合W3C标准的代码，能够根据交互原型和UI设计图完整制作出网页；
2.熟悉Javascript、css3和html5，且能熟练运用JQuery框架实现网页常用特效，掌握面向对象编程思想；
3.熟练应用dom、xml、json等相关技术；
4.熟悉Bootstrap前端框架，了解Nodejs和Angularjs以及less，sass、git、github等技术和团队协作开发工具；
5.具备抗压能力、且有一定自学能力，能够熟练阅读使用中文API，英文API可以大概看懂并运用；
6.担任项目组长并组织团队开发过电商、企业和移动端网站前端项目；

做事谨慎细心,工作认真负责,具有高度的责任感,喜欢钻研开发中遇到的问题
已积累一定数量中小型项目开发经验。
有较强的自主编程能力及团队合作，团队交流能力。我对Web前端开发比较熟悉，善于快速学习并使用新技术。

工作中能吃苦肯钻研，能承受较强工作压力，注重长期稳定的发展机会、谈判及沟通协调能力强。强烈的工作责任心及优秀的问题分析与处理能力，强烈的团队协作意识、结果导向及成本控制意识强，并且从事的每项工作都能很好的完成。

希望善于总结，总结也是学习能力的一种体现，每次完成一个研发任务，完成一段代码，都应当有目的的跟踪该程序的应用状况和用户反馈，随时总结，找到不足，这样逐步提高，一个程序员才可能成长起来




待改进
1.在开发工作中欠缺全局思想，做开发是看一块做一块，欠缺整体到局部的思想，在今后的工作中要努力锻炼这种思想
2.在开发工作中欠缺深挖精神，只是用了已有的代码完成了工作，只知道是如何使用的，没有继续挖掘如何实现的，
知其然不知其所以然，在日后的工作中如何时间充裕的话去学习其背后的原理知识
3.学习vue3的组合api新思想、新特性，时刻紧跟新技术




总结
【工作产出】进入公司，从初入公司的小白到主动承担前端开发任务，从事前端新需求开发、前端代码重复代码的整改工作、旧系统项目重构以及bug处理任务，和同事配合工作完成前端需求并上线，且无线上问题。
【效率提升】主动学习前端新知识和新技术，学习vue3的组合api思想、新版路由管理、状态管理、reactive变量、globalProperties全局变量、keep-alive组件等一些新的特性，并把新知识和新技术所使用的思想应用于当前项目，对当前项目提出自己的观点与同事进行分析讨论，改进和优化项目。在完成日常工作的同时，提升项目的响应速度，提高用户使用体验，前端感官效果，减少代码冗余等
【团队贡献】向身边的同事学习宝贵的开发经验，逻辑思路，积极配合同事工作，高效完成工作。积极帮助新员工，提高新员工在团队中的融入度，快速融入团队。


在日常工作中主要负责项目的前端开发工作，主要包含新需求的开发，重构原有页面，以及需求的变更任务等。在开发过程中收获了很多，但我觉得自己最大的收获是体会到了交流和沟通的重要性，刚进公司参加开发那段时间，自己对沟通认识不够深刻，对功能模块的开发只是按照需求文档进行开发，很多细节的地方都没有考虑到，等把程序开发出来才发现自己开发出来的功能跟实际需求存在偏差，细节功能不够完善，使得程序不能正常的运行。
这就使我认识到沟通和交流非常重要，在项目的开发过程中需要不断的与同事或客户进行沟通交流，完善功能模块的细节需求，只有这样开发出来的程序才能少出bug，按照需求任务正常运行，才能与整个系统更好的融合。虽然在思想和工作上有了一定的进步，但与其他同事相比还存在着一定的差距，因此，在今后的工作中，需要进一步改进和完善。比如工作中存在粗心、考虑事情不周的缺点，应变能力、协调能力也还有提升的空间，希望在今后在点滴实践中努力完善提高自己，弥补不足。
在工作之余也没有忘记学习。向身边的同事学习宝贵的开发经验，逻辑思路，逐步提高工作效率。在新技术上面也没有懈怠，学习vue3的组合api思想、新版路由管理、状态管理、reactive变量、globalProperties全局变量、keep-alive组件等一些新的特性，为日后更好的工作做准备。
目前SmartDM项目前端仍旧是由多个系统组合起来的 导致每个页面都有自己的风格，建议使用iframe嵌入的我们其他项目都可以重构为vue的项目，这样系统就能做到相对统一。

2022年主要负责SmartDM新需求的开发、tianYan项目重构、bug处理以及【配置管理状态报告】的开发和高危漏洞的清理，
在做项目时，主要以vue为开发框架，elementUI为UI组件，echarts进行统计图的处理。
在使用它们开发需求的同时也在逐步增加对它们的熟练度，为日后开发更复杂的需求提供帮助
1.在以后的工作中不断学习技术知识，通过多看、多学、多问、多练不断提高自己的各项技能，在深度学习的同时也不忘更广度的学习新技术。
2.提高全局性思维，拿到一个需求时先从整体出发看那些功能或组件可以复用，避免写重复代码。同时也做好复用组件和复用功能的笔记，之后再用时可快速完成开发。
3.向身边的同事学习宝贵的开发经验，逻辑思路，逐步提高工作效率。

个人计划: 
1.在以后的工作中不断学习新技术、新技能，在深度学习的同时也不忘更广度的学习新技术。
2.提高全局性思维，拿到一个需求时先从整体出发看那些功能或组件可以复用，避免写重复代码，同时也做好复用组件和复用功能的笔记，之后再使用时可快速完成开发。
3.在今后的工作中，也向身边的同事汲取宝贵的开发经验，逻辑思路。


