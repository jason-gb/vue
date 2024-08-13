vbase <template>
    <div>
        <!-- <h3>1. 기본 디렉티브</h3> -->
         <!-- <h3 v-text="title"></h3> -->
          <h3 v-html="title"></h3>
          <!-- <img v-bind:src="imgPath" width="300px"> -->
          <img :src="imgPath" width="300px">
          
          <div>
            <lable for="userId">이름</lable>
            <!-- <input type="text" id="userId" :value="name"> -->
            <!-- <input type="text" id="userId" v-model="name"> -->
            <!-- <input type="text" id="userId" v-model.lazy="name"> -->
            <input type="text" id="userId" v-model.trim.lazy="name">
            <br>

            <label for="">나이: </label>
            <!-- 숫자로 변환 가능한 값은 숫자로 변환하고 그렇지 않은 값은 문자열로 받아낸다 -->
            <input type="number" id="age" v-model.number="age">
            <br>

            <span>실행</span>
            <label><input type="radio" name="gender" v-model="gender">남자</label>
            <label><input type="radio" name="gender" v-model="gender">여자</label>
          </div>
    </div>
</template>

<script>
    export default {
        name: 'Directive1',
        data(){
            return {
                title : '<i>1. 기본 디렉티브</i>',
                imgPath : 'https://search.pstatic.net/common/?src=http%3A%2F%2Fblogfiles.naver.net%2FMjAyMjAzMjVfMjgz%2FMDAxNjQ4MTg3MDA2ODkz.R2gQHVrRiQaDp6y7IADZHwNrpWT_Z8lfX4WgjB8hEPsg.7IbPj82gBQxPM-NNhl3fjWxznuH_lec-M8hOknf_zB0g.JPEG.sosohan_n%2FIMG_6403.JPG&type=sc960_832',
                name : '홍길동'
            }
        }
    }
</script>