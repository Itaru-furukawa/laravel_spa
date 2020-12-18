<template>
    <div class="container">
        <div class="row justify-content-center">
            <div class="col-sm-6">
                <form>
                    <div class="label_block">
                        <label for="reqYear">扱い社名</label>
                        <select id="reqYear" class="form-control">
                            <option selected>株式会社セレスト</option>
                            <option>株式会社ジャストセレモニー</option>
                            <option>株式会社葬祭センター</option>
                        </select>
                    </div>
                    <div class="label_top">依頼年月日</div>
                    <div class="form-row">
                        <div class="form-group col-md-4">
                            <label for="reqYear">年</label>
                            <select id="reqYear" class="form-control">
                                <option selected>Choose...</option>
                                <option v-for="n in 20">{{ n + 2005}}</option>
                            </select>
                        </div>
                        <div class="form-group col-md-4">
                            <label for="reqMonth">月</label>
                            <select id="reqMonth" class="form-control">
                                <option selected>Choose...</option>
                                <option v-for="n in 12">{{ n }}</option>
                            </select>
                        </div>
                        <div class="form-group col-md-4">
                            <label for="reqDay">日</label>
                            <select id="reqDay" class="form-control">
                                <option selected>Choose...</option>
                                <option v-for="n in 31">{{ n }}</option>
                            </select>
                        </div>
                    </div>
                    <div class="label_top">通夜式</div>
                    <div class="form-row">
                        <div class="form-group col-md-4">
                            <label for="tuyaYear">年</label>
                            <select id="tuyaYear" class="form-control">
                                <option selected>Choose...</option>
                                <option v-for="n in 20">{{ n + 2005}}</option>
                            </select>
                        </div>
                        <div class="form-group col-md-4">
                            <label for="tuyaMonth">月</label>
                            <select id="tuyaMonth" class="form-control">
                                <option selected>Choose...</option>
                                <option v-for="n in 12">{{ n }}</option>
                            </select>
                        </div>
                        <div class="form-group col-md-4">
                            <label for="tuyaDay">日</label>
                            <select id="tuyaDay" class="form-control">
                                <option selected>Choose...</option>
                                <option v-for="n in 31">{{ n }}</option>
                            </select>
                        </div>
                        <div class="form-group col-md-4">
                            <label for="tuyaHour">開始時</label>
                            <select id="tuyaHour" class="form-control">
                                <option selected>Choose...</option>
                                <option v-for="n in 24">{{ n - 1 }}</option>
                            </select>
                        </div>
                        <div class="form-group col-md-4">
                            <label for="tuyaDay">開始分</label>
                            <select id="tuyaDay" class="form-control">
                                <option selected>Choose...</option>
                                <option v-for="n in 11">{{ n*5 }}</option>
                            </select>
                        </div>
                        <div class="form-group col-md-4">
                            <label for="tuyaHour">終了時</label>
                            <select id="tuyaHour" class="form-control">
                                <option selected>Choose...</option>
                                <option v-for="n in 24">{{ n - 1 }}</option>
                            </select>
                        </div>
                        <div class="form-group col-md-4">
                            <label for="tuyaDay">終了分</label>
                            <select id="tuyaDay" class="form-control">
                                <option selected>Choose...</option>
                                <option v-for="n in 11">{{ n*5 }}</option>
                            </select>
                        </div>
                        <div class="form-group col-md-4">
                            <label for="tuyaHour">集合時</label>
                            <select id="tuyaHour" class="form-control">
                                <option selected>Choose...</option>
                                <option v-for="n in 24">{{ n - 1 }}</option>
                            </select>
                        </div>
                        <div class="form-group col-md-4">
                            <label for="tuyaDay">集合分</label>
                            <select id="tuyaDay" class="form-control">
                                <option selected>Choose...</option>
                                <option v-for="n in 11">{{ n*5 }}</option>
                            </select>
                        </div>
                    </div>
                    <div class="label_top">告別式</div>
                    <div class="form-row">
                        <div class="form-group col-md-4">
                            <label for="tuyaYear">年</label>
                            <select id="tuyaYear" class="form-control">
                                <option selected>Choose...</option>
                                <option v-for="n in 20">{{ n + 2005}}</option>
                            </select>
                        </div>
                        <div class="form-group col-md-4">
                            <label for="tuyaMonth">月</label>
                            <select id="tuyaMonth" class="form-control">
                                <option selected>Choose...</option>
                                <option v-for="n in 12">{{ n }}</option>
                            </select>
                        </div>
                        <div class="form-group col-md-4">
                            <label for="tuyaDay">日</label>
                            <select id="tuyaDay" class="form-control">
                                <option selected>Choose...</option>
                                <option v-for="n in 31">{{ n }}</option>
                            </select>
                        </div>
                        <div class="form-group col-md-4">
                            <label for="tuyaHour">開始時</label>
                            <select id="tuyaHour" class="form-control">
                                <option selected>Choose...</option>
                                <option v-for="n in 24">{{ n - 1 }}</option>
                            </select>
                        </div>
                        <div class="form-group col-md-4">
                            <label for="tuyaDay">開始分</label>
                            <select id="tuyaDay" class="form-control">
                                <option selected>Choose...</option>
                                <option v-for="n in 11">{{ n*5 }}</option>
                            </select>
                        </div>
                        <div class="form-group col-md-4">
                            <label for="tuyaHour">終了時</label>
                            <select id="tuyaHour" class="form-control">
                                <option selected>Choose...</option>
                                <option v-for="n in 24">{{ n - 1 }}</option>
                            </select>
                        </div>
                        <div class="form-group col-md-4">
                            <label for="tuyaDay">終了分</label>
                            <select id="tuyaDay" class="form-control">
                                <option selected>Choose...</option>
                                <option v-for="n in 11">{{ n*5 }}</option>
                            </select>
                        </div>
                        <div class="form-group col-md-4">
                            <label for="tuyaHour">集合時</label>
                            <select id="tuyaHour" class="form-control">
                                <option selected>Choose...</option>
                                <option v-for="n in 24">{{ n - 1 }}</option>
                            </select>
                        </div>
                        <div class="form-group col-md-4">
                            <label for="tuyaDay">集合分</label>
                            <select id="tuyaDay" class="form-control">
                                <option selected>Choose...</option>
                                <option v-for="n in 11">{{ n*5 }}</option>
                            </select>
                        </div>
                    </div>
                    <div class="label_top">火葬式</div>
                    <div class="form-row">
                        <div class="form-group col-md-4">
                            <label for="tuyaYear">年</label>
                            <select id="tuyaYear" class="form-control">
                                <option selected>Choose...</option>
                                <option v-for="n in 25">{{ n + 2000}}</option>
                            </select>
                        </div>
                        <div class="form-group col-md-4">
                            <label for="tuyaMonth">月</label>
                            <select id="tuyaMonth" class="form-control">
                                <option selected>Choose...</option>
                                <option v-for="n in 12">{{ n }}</option>
                            </select>
                        </div>
                        <div class="form-group col-md-4">
                            <label for="tuyaDay">日</label>
                            <select id="tuyaDay" class="form-control">
                                <option selected>Choose...</option>
                                <option v-for="n in 31">{{ n }}</option>
                            </select>
                        </div>
                        <div class="form-group col-md-4">
                            <label for="tuyaHour">開始時</label>
                            <select id="tuyaHour" class="form-control">
                                <option selected>Choose...</option>
                                <option v-for="n in 24">{{ n - 1 }}</option>
                            </select>
                        </div>
                        <div class="form-group col-md-4">
                            <label for="tuyaDay">開始分</label>
                            <select id="tuyaDay" class="form-control">
                                <option selected>Choose...</option>
                                <option v-for="n in 11">{{ n*5 }}</option>
                            </select>
                        </div>
                        <div class="form-group col-md-4">
                            <label for="tuyaHour">終了時</label>
                            <select id="tuyaHour" class="form-control">
                                <option selected>Choose...</option>
                                <option v-for="n in 24">{{ n - 1 }}</option>
                            </select>
                        </div>
                        <div class="form-group col-md-4">
                            <label for="tuyaDay">終了分</label>
                            <select id="tuyaDay" class="form-control">
                                <option selected>Choose...</option>
                                <option v-for="n in 11">{{ n*5 }}</option>
                            </select>
                        </div>
                        <div class="form-group col-md-4">
                            <label for="tuyaHour">集合時</label>
                            <select id="tuyaHour" class="form-control">
                                <option selected>Choose...</option>
                                <option v-for="n in 24">{{ n - 1 }}</option>
                            </select>
                        </div>
                        <div class="form-group col-md-4">
                            <label for="tuyaDay">集合分</label>
                            <select id="tuyaDay" class="form-control">
                                <option selected>Choose...</option>
                                <option v-for="n in 11">{{ n*5 }}</option>
                            </select>
                        </div>
                    </div>
                    <div class="info_tag">故人様の情報</div>
                    <div class="moshu">
                        <div class="label_block">
                            <div class="form-group">
                                <label for="inputSouka">喪家名（よみかた）</label>
                                <input type="text" class="form-control" id="inputSouka" placeholder="ときわだい">
                            </div>
                            <div class="form-group">
                                <label for="inputAddress2">喪家名</label>
                                <input type="text" class="form-control" id="inputSouka2" placeholder="常盤台">
                            </div>
                            <div class="form-group">
                                <label for="inputAddress">故人名（よみかた）</label>
                                <input type="text" class="form-control" id="inputSouka" placeholder="ときわだい">
                            </div>
                            <div class="form-group">
                                <label for="inputAddress2">故人名</label>
                                <input type="text" class="form-control" id="inputSouka2" placeholder="常盤台">
                            </div>
                            <div class="form-group">
                                <label for="inputAddress2">住民登録地</label>
                                <input type="text" class="form-control" id="inputSouka2" placeholder="常盤台">
                            </div>
                            <div class="form-group">
                                <label for="inputAddress2">世帯主</label>
                                <input type="text" class="form-control" id="inputSouka2" placeholder="常盤台">
                            </div>
                            <div class="form-group">
                                <label for="inputAddress2">本籍地</label>
                                <input type="text" class="form-control" id="inputSouka2" placeholder="常盤台">
                            </div>
                            <div class="form-group">
                                <label for="inputAddress2">筆頭者</label>
                                <input type="text" class="form-control" id="inputSouka2" placeholder="常盤台">
                            </div>
                            
                        </div>
                        <div class="label_top">配偶者</div>
                        <div class="form-row">
                            <div class="form-group col-md-4 radio_spouse">
                                <input type="radio" checked id="one" value="exist" v-model="spouse">
                                <label for="one">いる</label>
                                <br>
                                <input type="radio"id="two" value="nexist" v-model="spouse">
                                <label for="two">いない</label>
                            </div>
                            <div class="form-group col-md-4" v-if="spouse === 'exist'">
                                <label for="spouseAge">満年齢</label>
                                <input type="number" class="form-control" id="spouseAge">
                            </div>
                            <div class="form-group col-md-4" v-else>
                                <label for="reqDay">状況</label>
                                <select id="reqDay" class="form-control">
                                    <option selected>未婚</option>
                                    <option>死別</option>
                                    <option>離別</option>
                                </select>
                            </div>
                        </div>
                        <div class="label_top">生年月日（故人）</div>
                        <div class="form-row">
                            <div class="form-group col-md-4">
                                <label for="tuyaYear">年</label>
                                <input type="number" class="form-control" id="inputAge1" placeholder="1960" v-model="birthYear">
                            </div>
                            <div class="form-group col-md-2">
                                <label for="tuyaMonth">月</label>
                                <input type="number" class="form-control" id="inputAge2" placeholder="1" v-model="birthMonth">
                            </div>
                            <div class="form-group col-md-2">
                                <label for="tuyaDay">日</label>
                                <input type="number" class="form-control" id="inputAge3" placeholder="20" v-model="birthDay">
                            </div>
                            <div class="age_form">満{{age}}歳</div>
                        </div>
                        <div class="label_top">性別</div>
                        <div class="form-group col-md-4 radio_spouse sex">
                            <input type="radio" checked id="male" value="male" v-model="sex">
                            <label for="male">男性</label>
                            <input type="radio"id="female" value="female" v-model="sex">
                            <label for="female">女性</label>
                        </div>
                        <div class="label_top">死亡したとき</div>
                        <div class="form-row">
                            <div class="form-group col-md-4">
                                <label for="tuyaYear">年</label>
                                <select id="tuyaYear" class="form-control" v-model="dead_year">
                                    <option>Choose...</option>
                                    <option v-for="n in 15" :value="todayYear -15 + n">{{ todayYear -15 + n}}</option>
                                </select>
                            </div>
                            <div class="form-group col-md-4">
                                <label for="tuyaMonth">月</label>
                                <select id="tuyaMonth" class="form-control" v-model="dead_month">
                                    <option>Choose...</option>
                                    <option v-for="i in 12" :value="i">{{i}}</option>
                                </select>
                            </div>
                            <div class="form-group col-md-4">
                                <label for="tuyaDay">日</label>
                                <select id="tuyaDay" class="form-control" v-model="dead_day">
                                    <option>Choose...</option>
                                    <option v-for="i in 31" :value="i">{{i}}</option>
                                </select>
                            </div>
                            <div class="form-group col-md-4">
                                <label for="tuyaHour">時</label>
                                <select id="tuyaHour" class="form-control">
                                    <option selected>Choose...</option>
                                    <option v-for="n in 24">{{ n - 1 }}</option>
                                </select>
                            </div>
                            <div class="form-group col-md-4">
                                <label for="tuyaDay">分</label>
                                <select id="tuyaDay" class="form-control">
                                    <option selected>Choose...</option>
                                    <option v-for="n in 11">{{ n*5 }}</option>
                                </select>
                            </div>
                        </div>
                    </div>
                    <div class="info_tag">喪主様の情報</div>
                    <div class="moshu">
                        <div class="label_block">
                            <div class="form-group">
                                <label for="inputSouka">喪主名（よみかた）</label>
                                <input type="text" class="form-control" id="inputSouka" placeholder="ときわだい">
                            </div>
                            <div class="form-group">
                                <label for="inputAddress2">喪主名</label>
                                <input type="text" class="form-control" id="inputSouka2" placeholder="常盤台">
                            </div>
                        </div>
                        <div class="label_top">生年月日（喪主）</div>
                        <div class="form-row">
                            <div class="form-group col-md-4">
                                <label for="tuyaYear">年</label>
                                <input type="number" class="form-control" id="inputAge1" placeholder="1960" v-model="birthYear">
                            </div>
                            <div class="form-group col-md-2">
                                <label for="tuyaMonth">月</label>
                                <input type="number" class="form-control" id="inputAge2" placeholder="1" v-model="birthMonth">
                            </div>
                            <div class="form-group col-md-2">
                                <label for="tuyaDay">日</label>
                                <input type="number" class="form-control" id="inputAge3" placeholder="20" v-model="birthDay">
                            </div>
                            <div class="age_form">満{{age}}歳</div>
                        </div>
                        <div class="label_block">
                            <div class="form-group">
                                <label for="inputAddress">続柄</label>
                                <input type="text" class="form-control col-md-2" placeholder="夫" v-model="relation">
                            </div>
                            <div>
                                <div class="form-group">
                                    <label for="inputAddress">電話番号</label>
                                    <input type="text" class="form-control" placeholder="03-0000-0000" v-model="tel">
                                </div>
                                <div class="form-group">
                                    <label for="inputAddress">携帯電話</label>
                                    <input type="text" class="form-control" placeholder="03-0000-0000" v-model="tel">
                                </div>
                            </div>
                            <div class="form-group">
                                <label for="inputAddress2">住民登録地</label>
                                <input type="text" class="form-control" id="inputSouka2" placeholder="常盤台">
                            </div>
                            <div class="form-group">
                                <label for="inputAddress2">世帯主</label>
                                <input type="text" class="form-control" id="inputSouka2" placeholder="常盤台">
                            </div>
                            <div class="form-group">
                                <label for="inputAddress2">本籍地</label>
                                <input type="text" class="form-control" id="inputSouka2" placeholder="常盤台">
                            </div>
                            <div class="form-group">
                                <label for="inputAddress2">筆頭者</label>
                                <input type="text" class="form-control" id="inputSouka2" placeholder="常盤台">
                            </div>
                        </div>
                    </div>
                    <div class="info_tag">届出人様の情報</div>
                    <div class="moshu">
                        <div class="label_block">
                            <div class="form-group">
                                <label for="inputSouka">届出人名（よみかた）</label>
                                <input type="text" class="form-control" id="inputSouka" placeholder="ときわだい">
                            </div>
                            <div class="form-group">
                                <label for="inputAddress2">届出人名</label>
                                <input type="text" class="form-control" id="inputSouka2" placeholder="常盤台">
                            </div>
                        </div>
                        <div class="label_top">生年月日（届出人）</div>
                        <div class="form-row">
                            <div class="form-group col-md-4">
                                <label for="tuyaYear">年</label>
                                <input type="number" class="form-control" id="inputAge1" placeholder="1960" v-model="birthYear">
                            </div>
                            <div class="form-group col-md-2">
                                <label for="tuyaMonth">月</label>
                                <input type="number" class="form-control" id="inputAge2" placeholder="1" v-model="birthMonth">
                            </div>
                            <div class="form-group col-md-2">
                                <label for="tuyaDay">日</label>
                                <input type="number" class="form-control" id="inputAge3" placeholder="20" v-model="birthDay">
                            </div>
                            <div class="age_form">満{{age}}歳</div>
                        </div>
                        <div class="label_block">
                            <div class="form-group">
                                <label for="inputAddress">続柄</label>
                                <input type="text" class="form-control col-md-2" placeholder="夫" v-model="relation">
                            </div>
                            <div>
                                <div class="form-group">
                                    <label for="inputAddress">電話番号</label>
                                    <input type="text" class="form-control" placeholder="03-0000-0000" v-model="tel">
                                </div>
                                <div class="form-group">
                                    <label for="inputAddress">携帯電話</label>
                                    <input type="text" class="form-control" placeholder="03-0000-0000" v-model="tel">
                                </div>
                            </div>
                            <div class="form-group">
                                <label for="inputAddress2">住民登録地</label>
                                <input type="text" class="form-control" id="inputSouka2" placeholder="常盤台">
                            </div>
                            <div class="form-group">
                                <label for="inputAddress2">世帯主</label>
                                <input type="text" class="form-control" id="inputSouka2" placeholder="常盤台">
                            </div>
                            <div class="form-group">
                                <label for="inputAddress2">本籍地</label>
                                <input type="text" class="form-control" id="inputSouka2" placeholder="常盤台">
                            </div>
                            <div class="form-group">
                                <label for="inputAddress2">筆頭者</label>
                                <input type="text" class="form-control" id="inputSouka2" placeholder="常盤台">
                            </div>
                        </div>
                    </div>
                    <div class="info_tag">請求情報</div>
                    <div class="moshu">
                        <div class="label_block">
                            <div class="form-group">
                                <label for="inputAddress">請求先名</label>
                                <input type="text" class="form-control" id="inputSouka2" placeholder="常盤台">
                            </div>
                            <div>
                                <div class="form-group">
                                    <label for="inputAddress">電話番号</label>
                                    <input type="text" class="form-control" placeholder="03-0000-0000" v-model="tel">
                                </div>
                            </div>
                            <div class="form-group">
                                <label for="inputAddress2">請求先ご住所</label>
                                <input type="text" class="form-control" id="inputSouka2" placeholder="常盤台">
                            </div>
                            
                        </div>
                        <div class="label_top">精算方法</div>
                        <div class="form-group pay_way">
                            <input type="radio" value="振込" id="pay1" v-model="pay_way">
                            <label for="pay1">振込</label>
                            <input type="radio" value="集金" id="pay2" v-model="pay_way">
                            <label for="pay2">集金</label>
                            <input type="radio" value="当日" id="pay3" v-model="pay_way">
                            <label for="pay3">当日</label>
                        </div>
                    </div>
                    <div class="info_tag">その他</div>
                    <div class="moshu">
                        <div class="label_block">
                            <div class="form-group">
                                <label for="inputAddress">式場名</label>
                                <select class="form-control">
                                    <option></option>
                                </select>
                            </div>
                            <div class="form-group">
                                <label for="inputAddress">式場住所</label>
                                <input readonly type="text" class="form-control">
                            </div>
                            <div class="form-group">
                                <label for="inputAddress">式場電話番号</label>
                                <input readonly type="text" class="form-control">
                            </div>
                            <div class="form-group">
                                <label for="inputAddress">火葬場</label>
                                <input type="text" class="form-control">
                            </div>
                            <div class="form-group">
                                <label for="inputAddress">宗派・寺院名</label>
                                <input type="text" class="form-control">
                            </div>
                            <div class="form-group">
                                <label for="inputAddress">御布施</label>
                                <input type="text" class="form-control">
                            </div>
                            <div class="form-group">
                                <label for="inputAddress">返礼品</label>
                                <input type="text" class="form-control">
                            </div>
                            <div class="form-group">
                                <label for="inputAddress">特筆事項</label>
                                <div>
                                    <textarea placeholder="Enterで改行することができます" class="col-md-12"></textarea>
                                </div>
                            </div>
                        </div>
                    </div>
                    
                    <button type="submit" class="btn btn-primary btn-lg btn-block">入力完了</button>
                </form>
            </div>
        </div>
    </div>
</template>

<script>
import moment from 'moment';
export default {
    data() {
        return {
            sex :'male',
            spouse :'exist',
            dead_month: '12',
            date : moment(),
            todayYear: moment().format('YYYY'),
            dead_year: moment().format('YYYY'),
            dead_month: moment().format('MM'),
            dead_day: moment().format('DD'),
            today : moment().format(),
            birthYear : '1950',
            birthMonth : '01' ,
            birthDay : '01',
            pay_way : '振込',
        };
    },
    computed: {
        double() {
        return this.number * 2;
        },
        numberClass() {
        if (this.number > 50) {
            return "red";
        }

        return "blue";
        },
        age(){
            return moment().diff(this.birthYear + '-' + this.birthMonth + '-' + this.birthDay, 'years');
        }

    },
    filters: {
        moment: function (date) {
            return moment(date).format('YYYY/MM/DD HH:mm');
        }
    },
    methods: {
        add(val) {
        this.number = this.number + val;
        },
        toInt: function(val){
            return parseInt(val);
        }
    }
};
</script>

<style>
    form{
        margin-bottom:200px;
    }
    .label_top{
        margin-top:20px;
        font-weight:bold;
        font-size :17px;
    }
    .label_block label{
        font-size:17px;
        font-weight: bold;
    }
    .radio_spouse{
        margin-top: 10px;
    }
    .age_form{
        font-size :18px;
        padding-top: 35px;
        margin-left: 30px;
    }
    .sex{
        font-size :17px;
    }
    .sex label{
        margin-right: 5px;
    }
    .moshu{
        border:1px solid #dadada;
        padding: 20px;
        margin-bottom:50px;
    }
    .pay_way{
        font-size:18px;
    }
    .pay_way input{
        margin-left:20px;
    }
    .info_tag{
        font-size:20px;
    }
</style>