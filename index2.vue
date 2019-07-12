<template>
  <div class="container">
    <div>
      <h1 class="title">
        exceed-starter
      </h1>
      <h2 class="subtitle">
        Mind over matter
      </h2>
      <div class="links">
        <a
          href="https://nuxtjs.org/"
          target="_blank"
          class="button--green"
        >
          Documentation
        </a>
        <a
          href="https://github.com/nuxt/nuxt.js"
          target="_blank"
          class="button--grey"
        >
          GitHub
        </a>
      </div>
      <div v-for="question in questions" :key="question.ID">
        Item #<span>{{ question.ID }}</span>
      </div>
      <div>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus officia molestias itaque temporibus qui nihil, dolor eos perspiciatis nobis voluptatem quidem odio similique, architecto voluptas fugiat, enim iste ab tempora.
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Officiis repudiandae sapiente ut, explicabo dicta, vitae obcaecati error possimus inventore natus modi laborum dolores suscipit quod debitis. Sint, sunt. Aperiam, dolore.
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Assumenda itaque asperiores dolor unde numquam aliquam enim aspernatur impedit deserunt aut esse cumque eum distinctio, animi autem saepe quas ipsam sunt?
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Maiores quaerat dolorem natus vitae sequi suscipit, recusandae sint veniam laboriosam dicta nulla ipsa qui blanditiis excepturi, iusto possimus accusamus commodi dolore!
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Impedit sequi illum dolorum ratione neque hic magnam quos labore fuga suscipit doloremque ad incidunt tempore, assumenda aspernatur accusantium officia blanditiis ut.
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium ipsa eius, dicta modi praesentium necessitatibus accusamus consectetur quas magnam et deleniti! Odio ad hic consequatur debitis praesentium dolore libero labore!
        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Praesentium molestias esse, dolorem culpa dignissimos iste doloremque inventore commodi numquam itaque, voluptatibus consectetur nisi aperiam vero nihil eaque tempore perspiciatis a!
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Sunt voluptas quod at a omnis, aut doloribus ad! Vitae facere porro cum delectus odio, assumenda aliquid neque, dolores voluptas vero tempore.
      </div>
    </div>
  </div>
</template>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>




<!---start!!!!!111111111111111-->
<script>
export default {
  data: ()=> {
    return {
     four_day_data:'take from database',//not write fn to insert data from database yet!!!!!!!!!!!!!!!! structure [[light,moving].......]
     emergency_status='off' ,
     calling_status='off',
     status_of_patient='' ,
     questions: [
        { answer: [''], ID: 1 },
        { answer: [''], ID: 2 },
        { answer: [''], ID: 3 },
        { answer: [''], ID: 4 },
        { answer: [''], ID: 5 },
        { answer: [''], ID: 6 },
        { answer: [''], ID: 7 },
        { answer: [''], ID: 8 },
        { answer: [''], ID: 9 },
        {sleeping_time}
     ]
    },
  methods; {
    check_box();{
        this.questions[0].answer
    }

    

     //not ready yet!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
    next_btn(before_html,next_html);{
       var next_html = document.getElementById("myH2");
       next_html.insertAdjacentHTML("afterend", "<p>My new paragraph</p>");
       var before_html = document.getElementById(selectorID);
       before_html.parentNode.removeChild(before_html);
     },
    
    
    check_psyco();{
      tend_psyco_score=0
      for( var i=0;i<4;i++){
        //darkplace totalscore
        if(this.four_day_data[i][0]>3 && darkplace[i][0]<5){
          tend_psyco_score+=1
        }
        elif(this.four_day_data[i][0]>5 &&this.four_day_data[i][0]<7){                                                                           
          tend_psyco_score+=2
        }
        elif(this.four_day_data[i][0]>7){
          tend_psyco_score+=3
        }
        else()=>{
          pass
        }


        //moving
        if(this.four_day_data[i][1]>3 && this.four_day_data[i][1]<5){
          tend_psyco_score+=1}
        elif(this.four_day_data[i][1]>5 && this.four_day_data[i][1]<7){
          tend_psyco_score+=2}
        elif(dthis.four_day_data[i][1]>7){
          tend_psyco_score+=3}
        else()=>{
          pass
        }
      }

      //check psysco
      if(tend_psyco_score<5){
        status_of_patient= 'ปกติ'
      }
      elif(tend_psyco_score<10);{
        status_of_patient= 'ซึมเศร้าขั้นต้น'
      }
      elif(tend_psyco_score<10);{
        status_of_patient='ซึมเศร้าปานกลาง'
      }
      elif(tend_psyco_score<10);{
        status_of_patient='ซึมเศร้ารุนแรง'
        emergency_status='on'
      }
    },
    // function get the data from server

    submit_all() {
      if (checked.lenght != 9 ){
        alert('please enter all questions')
       }
      else{
        const checked = document.querySelectorAll('input[checked]')
        for (const checkbox of checked) sum+= Number.parseInt(checkbox.value)
          if (scroe<7){
            status_of_patient='ไม่เป็นโรคซึมเศร้า'
          }
          elif (score<12 && score>7);{
            status_of_patient = 'ระดับน้อย'}
          elif (score<18 && score>13);{
            status_of_patient = 'ระดับปานกลาง'}
          elif (score<18 && score>13);{
            status_of_patient = 'ระดับรุนแรง'}
          else {
            status_of_patient = 'เป็นโรคซึมเศร้ารุนเรง'
          }
                   // return value to server!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! return status_of_patient ,x =documrnt.queryselector('').value
    }
    status_in_doctor_panel(){


        
      if (this.calling_status ==='on'){
        document.getElementById('call').style = 'background-color:red;color:red'
      }
      if (this.emergency_status ==='on'){
        document.getElementsById('emergency').style = 'background-color:red;color:red'
      }
      if (this.status_of_patient==='ระดับน้อย'){
        document.querySelector('btn btn-primary') = 'ระดับน้อย'
        document.getElementById('btn btn-primary').style.backgroundColor='green';
      }
      elif(this.status_of_patient==='ระดับปานกลาง'){
        document.querySelector('btn btn-primary') = 'ระดับปานกลาง'
        document.getElementById('btn btn-primary').style.backgroundColor='yellow';
      }
      elif(this.status_of_patient === 'ระดับรุนแรง'){
        document.querySelector('btn btn-primary') = 'ระดับรุนแรง'
        document.getElementById('btn btn-primary').style.backgroundColor='red';

      }

    }




    


    }
   }
  }
}
</script>
