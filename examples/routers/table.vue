<template>
    <Table
      :data="tableData"
      style="width: 100%">
      <Column
        prop="date"
        label="日期"
        width="180">
      </Column>
      <Column :filters="[{ text: '家', value: '家' }, { text: '公司', value: '公司' }]"

      filter-placement="bottom-end"
        prop="name"
        label="姓名"
        width="180">
      </Column>
      <Column column-key="aaaaa" 
        prop="address"
        label="地址">
      </Column>
    </Table>
  </template>

  <script>
    export default {
      data() {
        return {
          tableData: [{
            date: '2016-05-02',
            name: '王小虎',
            address: '上海市普陀区金沙江路 1518 弄'
          }, {
            date: '2016-05-04',
            name: '王小虎',
            address: '上海市普陀区金沙江路 1517 弄'
          }, {
            date: '2016-05-01',
            name: '王小虎',
            address: '上海市普陀区金沙江路 1519 弄'
          }, {
            date: '2016-05-03',
            name: '王小虎',
            address: '上海市普陀区金沙江路 1516 弄'
          }]
        }
      }
    }
  </script>
