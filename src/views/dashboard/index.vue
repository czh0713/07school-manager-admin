<template>
  <div class="dashboard-container">
      <div class="item">
        <h1>全校学生</h1>
        <h1>{{studentCount}}</h1>
      </div>
	  <div class="item">
        <h1>全校老师</h1>
        <h1>{{teacherCount}}</h1>
      </div>
	  <div class="item">
        <h1>全校班级</h1>
        <h1>{{classCount}}</h1>
      </div>
	

  </div>
</template>

<script>
  import { mapGetters } from 'vuex'

  export default {
    name: 'Dashboard',
    computed: {
      ...mapGetters([
        'name'
      ])
    },

    data(){
      return{
		students:'',
        studentCount:'',
		teacher:'',
        teacherCount:'',
		classs:'',
		classCount: ''

      }
    },
    mounted(){
		this.$http.post('/api/student/get').then(res => {
        this.students = res
		this.studentCount = this.students.length;
		console.log(this.studentCount);
		})
	
		this.$http.post('/api/teacher/get').then(res => {
        this.teacher = res
		this.teacherCount = this.teacher.length;
		console.log(this.teacherCount);
		})
		
		this.$http.post('/api/classs/get').then(res => {
        this.classs = res
		this.classCount = this.classs.length;
		console.log(this.classCount);
		})
	


    }
  }
</script>

<style lang="scss" scoped>
  .dashboard {
    &-container {
      margin: 30px;
    }
    &-text {
      font-size: 30px;
      line-height: 46px;
    }
  }

  .dashboard-container{
    display: flex;
  }
  .item{
    text-align: center;
    transition: all 0.3s;
    position: relative;
    border-radius: 3px;
    top: 0;
    box-shadow: 0 0 0 0 rgba(0,0,0,0.1);
    padding: 10px;
    margin: 10px;
  }
  .item:hover{
    top: -20;
    box-shadow: 1px 10px 15px 2px rgba(0,0,0,0.1);
  }
</style>
