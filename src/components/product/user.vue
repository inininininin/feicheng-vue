<template>

	<div class="user">
		<div v-if="loading" style="text-align:center;">
		  <img style="width:30px" src="../../assets/img/loading.png" />
	  	</div>
	<div v-if="!loading">
		<div class="first">
			<el-row class="user_name" :gutter='2' style="margin-bottom: 2px;">
				<el-col :xs="6" :sm="6" :md="6" :lg="6" :xl="6">
					<div class="user_quanxian">
						<div class="user_quanxian_banben">
							<div class="user_quanxian_banben_mianfei">
								<svg width="16" height="16" viewBox="0 0 16 16" class="_3s3MgTxZ"><defs><linearGradient id="linear-gradientll" x1="0.5" x2="0.5" y2="1" gradientUnits="objectBoundingBox"><stop offset="0" stop-color="#ebebeb"></stop><stop offset="1" stop-color="#a6a6a6"></stop></linearGradient><linearGradient id="linear-gradientmm" x1="0.5" x2="0.5" y2="1" gradientUnits="objectBoundingBox"><stop offset="0" stop-color="#ebebeb"></stop><stop offset="1" stop-color="#bfbfbf"></stop></linearGradient></defs><g id="\u7EC4_4034" data-name="\u7EC4 4034" transform="translate(-193.665 -1471.826)"><circle id="\u692D\u5706_122" data-name="\u692D\u5706 122" fill="url(#linear-gradientll)" cx="8" cy="8" r="8" transform="translate(193.665 1471.826)"></circle><g id="\u8DEF\u5F84_10109" data-name="\u8DEF\u5F84 10109" fill="url(#linear-gradientmm)" transform="translate(-199.308 61.299)"><path stroke="none" d="M404.948,1417.543a.808.808,0,0,0-.566-.493l-.012,0-1.685-.457-1.1-1.671-.006-.009a.79.79,0,0,0-.617-.382.723.723,0,0,0-.608.4l-.938,1.524-1.261.383-.615.187a.765.765,0,0,0-.537.447.9.9,0,0,0,.159.763l.014.021,1.1,1.4q-.028,1.007-.057,2.017a.922.922,0,0,0,.142.693.484.484,0,0,0,.387.165,1.416,1.416,0,0,0,.474-.105l1.622-.66,1.845.686a1.1,1.1,0,0,0,.333.059c.228,0,.616-.1.647-.808a.213.213,0,0,0,0-.022q-.051-.9-.1-1.8v-.008l1.2-1.607a.843.843,0,0,0,.182-.722Z"></path><path fill="rgba(255,255,255,0.65)" stroke="none" d="M 400.9640502929688 1414.526977539063 C 400.803466796875 1414.526977539063 400.568115234375 1414.59619140625 400.356201171875 1414.928833007813 L 399.4177856445313 1416.453125 C 398.9976196289063 1416.580444335938 398.577392578125 1416.708374023438 398.1570434570313 1416.836181640625 L 397.54248046875 1417.023071289063 C 397.2562866210938 1417.116088867188 397.0755004882813 1417.266479492188 397.0050659179688 1417.470336914063 C 396.9312133789063 1417.684448242188 396.9832153320313 1417.93408203125 397.1640014648438 1418.233764648438 C 397.1683349609375 1418.240844726563 397.1732177734375 1418.247924804688 397.1784057617188 1418.254516601563 C 397.5462036132813 1418.719970703125 397.9136962890625 1419.185546875 398.2810668945313 1419.651489257813 C 398.26220703125 1420.323120117188 398.2430419921875 1420.99560546875 398.2235717773438 1421.668090820313 C 398.195556640625 1421.989990234375 398.2421264648438 1422.216796875 398.3657836914063 1422.361572265625 C 398.45947265625 1422.471313476563 398.5897827148438 1422.52685546875 398.7530517578125 1422.52685546875 C 398.8782348632813 1422.52685546875 399.026611328125 1422.494262695313 399.2268676757813 1422.42138671875 L 400.8492431640625 1421.760986328125 C 401.4641723632813 1421.990234375 402.0792846679688 1422.218994140625 402.694580078125 1422.447143554688 C 402.815673828125 1422.486083984375 402.927734375 1422.505859375 403.0279541015625 1422.505859375 C 403.2562255859375 1422.505859375 403.6437377929688 1422.40087890625 403.6747436523438 1421.697387695313 C 403.675048828125 1421.690185546875 403.6749877929688 1421.682983398438 403.674560546875 1421.67578125 C 403.6405639648438 1421.076293945313 403.6063232421875 1420.478149414063 403.572021484375 1419.879638671875 L 403.571533203125 1419.871704101563 L 404.7665405273438 1418.264770507813 C 404.9508666992188 1417.999633789063 405.0120239257813 1417.756713867188 404.9481201171875 1417.543090820313 C 404.8826904296875 1417.324829101563 404.6922607421875 1417.159057617188 404.3819580078125 1417.050415039063 C 404.3779296875 1417.048950195313 404.3738403320313 1417.047729492188 404.3696899414063 1417.046508789063 L 402.6848754882813 1416.589477539063 C 402.3195190429688 1416.0322265625 401.95361328125 1415.475219726563 401.587890625 1414.918212890625 C 401.5863647460938 1414.915893554688 401.5830688476563 1414.910888671875 401.5814819335938 1414.908813476563 C 401.405517578125 1414.662475585938 401.1860961914063 1414.526977539063 400.9640502929688 1414.526977539063 M 400.9640502929688 1413.526977539063 C 401.5101318359375 1413.526977539063 402.0317687988281 1413.818725585938 402.3952026367188 1414.327514648438 L 402.39501953125 1414.327758789063 C 402.4059753417969 1414.343139648438 402.4176635742188 1414.359985351563 402.4243469238281 1414.370239257813 L 402.649658203125 1414.71337890625 C 402.8707885742188 1415.050048828125 403.0919494628906 1415.386840820313 403.3129577636719 1415.723754882813 L 404.6315002441406 1416.081420898438 L 404.6416320800781 1416.084106445313 L 404.6517333984375 1416.087158203125 C 404.6722717285156 1416.093139648438 404.6924133300781 1416.099609375 404.71240234375 1416.106567382813 L 404.71240234375 1416.106567382813 C 405.4964599609375 1416.381103515625 405.7942504882813 1416.883178710938 405.906005859375 1417.255981445313 C 406.0131225585938 1417.614013671875 406.044677734375 1418.178100585938 405.5876159667969 1418.835571289063 L 405.5784912109375 1418.848754882813 L 405.5689697265625 1418.861572265625 L 404.5906982421875 1420.177001953125 C 404.6182861328125 1420.658935546875 404.6457214355469 1421.138671875 404.6729736328125 1421.619140625 C 404.6752319335938 1421.657348632813 404.6755981445313 1421.69921875 404.6737976074219 1421.740356445313 C 404.6200561523438 1422.960327148438 403.8084716796875 1423.505859375 403.0279541015625 1423.505859375 C 402.8238525390625 1423.505859375 402.6086730957031 1423.469970703125 402.3884582519531 1423.399169921875 L 402.3675231933594 1423.392456054688 L 402.346923828125 1423.384765625 C 401.8529357910156 1423.201538085938 401.3590393066406 1423.01806640625 400.8652954101563 1422.834106445313 L 399.6038818359375 1423.34765625 L 399.5864868164063 1423.354614257813 L 399.56884765625 1423.361083984375 C 399.2580871582031 1423.474243164063 398.9988708496094 1423.52685546875 398.7530517578125 1423.52685546875 C 398.2969360351563 1423.52685546875 397.8893127441406 1423.343627929688 397.6052551269531 1423.010864257813 C 397.3081665039063 1422.662963867188 397.18017578125 1422.192749023438 397.2247619628906 1421.612915039063 C 397.2404479980469 1421.070434570313 397.2559509277344 1420.527954101563 397.271240234375 1419.985961914063 C 396.9788818359375 1419.615234375 396.6864318847656 1419.244873046875 396.393798828125 1418.87451171875 C 396.3636474609375 1418.836181640625 396.3362731933594 1418.796875 396.3114318847656 1418.75634765625 L 396.3095703125 1418.753295898438 L 396.3077392578125 1418.750366210938 C 395.9691467285156 1418.189086914063 395.8857116699219 1417.648681640625 396.0597534179688 1417.144287109375 C 396.1602172851563 1416.853393554688 396.4461059570313 1416.327880859375 397.2333984375 1416.072021484375 L 397.242431640625 1416.069091796875 L 397.2515258789063 1416.066284179688 L 397.8660888671875 1415.87939453125 L 398.1297912597656 1415.79931640625 C 398.3415222167969 1415.73486328125 398.5531921386719 1415.670532226563 398.764892578125 1415.606201171875 L 399.504638671875 1414.404541015625 L 399.5086669921875 1414.398071289063 L 399.5128173828125 1414.391479492188 C 399.9920349121094 1413.639282226563 400.6277465820313 1413.526977539063 400.9640502929688 1413.526977539063 Z"></path></g><path id="\u51CF\u53BB_4" data-name="\u51CF\u53BB 4" fill="#fff" stroke="rgba(0,0,0,0)" stroke-miterlimit="10" opacity="0.3" d="M1.78,8a.485.485,0,0,1-.387-.165.924.924,0,0,1-.142-.693q.028-.97.055-1.94V5.178l0-.054-1.1-1.4a.107.107,0,0,1-.013-.018.912.912,0,0,1-.161-.766A.768.768,0,0,1,.57,2.5l.615-.187,1.26-.383L3.383.4A.726.726,0,0,1,3.991,0a.79.79,0,0,1,.618.382l0,0,0,.006.272.413.825,1.257.376.1L3.344,7.451l-1.091.444A1.405,1.405,0,0,1,1.78,8Z" transform="translate(197.665 1475.826)"></path></g></svg>
						

								<span style="font-size: 14px;margin-left: 2px;vertical-align: text-bottom;"> {{ (!this.$store.state.wxVideoaccount || this.$store.state.wxVideoaccount.type==null)?"体验版"
                  :this.$store.state.wxVideoaccount.type==0?"体验版"
                  :this.$store.state.wxVideoaccount.type==1?"个人号"
                  :this.$store.state.wxVideoaccount.type==2?"达人号"
                  :this.$store.state.wxVideoaccount.type==3?"企业号"
                  :"未知" }}</span>



							</div>
							<!-- <div class="user_quanxian_banben_shezhi">
								<svg viewBox="64 64 896 896" focusable="false" class="" data-icon="setting" width="1em" height="1em" fill="currentColor" aria-hidden="true"><path d="M924.8 625.7l-65.5-56c3.1-19 4.7-38.4 4.7-57.8s-1.6-38.8-4.7-57.8l65.5-56a32.03 32.03 0 0 0 9.3-35.2l-.9-2.6a443.74 443.74 0 0 0-79.7-137.9l-1.8-2.1a32.12 32.12 0 0 0-35.1-9.5l-81.3 28.9c-30-24.6-63.5-44-99.7-57.6l-15.7-85a32.05 32.05 0 0 0-25.8-25.7l-2.7-.5c-52.1-9.4-106.9-9.4-159 0l-2.7.5a32.05 32.05 0 0 0-25.8 25.7l-15.8 85.4a351.86 351.86 0 0 0-99 57.4l-81.9-29.1a32 32 0 0 0-35.1 9.5l-1.8 2.1a446.02 446.02 0 0 0-79.7 137.9l-.9 2.6c-4.5 12.5-.8 26.5 9.3 35.2l66.3 56.6c-3.1 18.8-4.6 38-4.6 57.1 0 19.2 1.5 38.4 4.6 57.1L99 625.5a32.03 32.03 0 0 0-9.3 35.2l.9 2.6c18.1 50.4 44.9 96.9 79.7 137.9l1.8 2.1a32.12 32.12 0 0 0 35.1 9.5l81.9-29.1c29.8 24.5 63.1 43.9 99 57.4l15.8 85.4a32.05 32.05 0 0 0 25.8 25.7l2.7.5a449.4 449.4 0 0 0 159 0l2.7-.5a32.05 32.05 0 0 0 25.8-25.7l15.7-85a350 350 0 0 0 99.7-57.6l81.3 28.9a32 32 0 0 0 35.1-9.5l1.8-2.1c34.8-41.1 61.6-87.5 79.7-137.9l.9-2.6c4.5-12.3.8-26.3-9.3-35zM788.3 465.9c2.5 15.1 3.8 30.6 3.8 46.1s-1.3 31-3.8 46.1l-6.6 40.1 74.7 63.9a370.03 370.03 0 0 1-42.6 73.6L721 702.8l-31.4 25.8c-23.9 19.6-50.5 35-79.3 45.8l-38.1 14.3-17.9 97a377.5 377.5 0 0 1-85 0l-17.9-97.2-37.8-14.5c-28.5-10.8-55-26.2-78.7-45.7l-31.4-25.9-93.4 33.2c-17-22.9-31.2-47.6-42.6-73.6l75.5-64.5-6.5-40c-2.4-14.9-3.7-30.3-3.7-45.5 0-15.3 1.2-30.6 3.7-45.5l6.5-40-75.5-64.5c11.3-26.1 25.6-50.7 42.6-73.6l93.4 33.2 31.4-25.9c23.7-19.5 50.2-34.9 78.7-45.7l37.9-14.3 17.9-97.2c28.1-3.2 56.8-3.2 85 0l17.9 97 38.1 14.3c28.7 10.8 55.4 26.2 79.3 45.8l31.4 25.8 92.8-32.9c17 22.9 31.2 47.6 42.6 73.6L781.8 426l6.5 39.9zM512 326c-97.2 0-176 78.8-176 176s78.8 176 176 176 176-78.8 176-176-78.8-176-176-176zm79.2 255.2A111.6 111.6 0 0 1 512 614c-29.9 0-58-11.7-79.2-32.8A111.6 111.6 0 0 1 400 502c0-29.9 11.7-58 32.8-79.2C454 401.6 482.1 390 512 390c29.9 0 58 11.6 79.2 32.8A111.6 111.6 0 0 1 624 502c0 29.9-11.7 58-32.8 79.2z"></path></svg>
								<span>权限</span>
							</div> -->
						</div>
						<div class="user_message">
							<img :src="login? login.logo:require('../../assets/img/touxiang.png')" alt="">
							<h5>{{login? login.nickname:''}}</h5>
							<p v-if='!this.$store.state.wxVideoaccount ||  !this.$store.state.wxVideoaccount.type' style="font-size: 14px;">
								您还不是博主，
								<router-link :to="{path:'/product/ruzhu'}">
									<span>立即入驻</span>
								</router-link>
							</p>
							<p v-else>
								<!-- <span v-if='getUserInfo.audits==1'>等待审核</span>
								<span v-if='getUserInfo.audits==11'>已认证</span>
								<span @click='askIfEnter()' v-if='getUserInfo.audits==12'>认证失败</span> -->
								<span @click='askIfEnter()' >{{
									(!this.$store.state.wxVideoaccount|| this.$store.state.wxVideoaccount.audit==null)?""
									:this.$store.state.wxVideoaccount.audit==0?""
									:this.$store.state.wxVideoaccount.audit==1?"(审核中)"
									:this.$store.state.wxVideoaccount.audit==11?"(已认证)"
									:this.$store.state.wxVideoaccount.audit==12?"(认证失败)"
									:"未知" }}</span>
							</p>
							<p v-if="login? login.vipEndTime:false"> VIP于{{moment(this.$store.state.login.vipEndTime).format('YYYY-MM-DD hh:mm')}}到期</p>
						</div>	
						<div class="_1aHAtMPw _1xvNCILN"></div>
						<div class="_1aHAtMPw"></div>
					</div>
				</el-col>
				<el-col :xs="18" :sm="18" :md="18" :lg="18" :xl="18">
					<el-carousel height="300px">
						<el-carousel-item v-for="(item,inx) in list" :key="inx">
							<router-link :to="{path:item.url}"  target="_blank">
								<img :src="item.src" alt="" style="height:100%;width: 100%;">
							</router-link>
						</el-carousel-item>
					</el-carousel>
				</el-col>
			</el-row>
			<el-row class="uer_zhixun" :gutter='2'>
				<el-col :xs="6" :sm="6" :md="6" :lg="6" :xl="6">
					<div class="uer_zhixun_gongneng" style="position: relative;">
						<div class="uer_zhixun_gongneng_hezi uer_scroll" v-infinite-scroll="nextPageOne" :infinite-scroll-disabled="loadOne" infinite-scroll-distance="10">
							<div v-for="(item,inx) in articleOne" @click="detailClickFn(item)" :key="inx" style="width: 100%;padding:0px 5px;height: auto;box-sizing: border-box;overflow-x:hidden ;">
								<!-- <router-link target='_blank' :to="{path:'/articleDetails',query:{data:JSON.stringify(item)}}"> -->
									<span >{{item.name}}</span>
								<!-- </router-link> -->
							</div>

						</div>
						<div class="_sXxpqwDa">帮助</div>
					</div>
				</el-col>
				<el-col :xs="9" :sm="9" :md="9" :lg="9" :xl="9">
					<div class="uer_zhixun_tuisong "  style="position: relative;">
						<div class="uer_zhixun_tuisongList uer_scroll" v-infinite-scroll="nextPageTwo" :infinite-scroll-disabled="loadTwo" infinite-scroll-distance="10">
							<div class="uer_zhixun_tuisongList_hezhi" @click="detailClickFn(item)" v-for="(item,inx) in articleTwo" :key="inx">
								<!-- <router-link target='_blank' :to="{path:'/articleDetails',query:{data:JSON.stringify(item)}}"> -->
									<p>
										<span>{{moment(item.createTime).format('YYYY-MM-DD')}}</span>
										{{item.name}}
									</p>
									<p>{{item.brief}}</p>
								</router-link>
							</div>

							<!-- <span>查看更多 ></span> -->
						</div>
						<div class="_sXxpqwDa">公告</div>
					</div>
				</el-col>
				<el-col :xs="9" :sm="9" :md="9" :lg="9" :xl="9">
					<div class="uer_zhixun_lishi "   style="position: relative;">
						<div class="uer_zhixun_lishiList uer_scroll" v-infinite-scroll="nextPageThree" :infinite-scroll-disabled="loadThree" infinite-scroll-distance="10">
							<div class="uer_zhixun_lishiList_hezhi" @click="detailClickFn(item)" v-for="(item,inx) in articleThree" :key="inx">
								<!-- <router-link target='_blank' :to="{path:'/articleDetails',query:{data:JSON.stringify(item)}}"> -->
								<div class="ant-timeline-item-tail" v-if="item.data"></div>
								<div class="ant-timeline-item-head ant-timeline-item-head-gray" ></div>
									<div class="uer_zhixun_lishiList_hezhi_neirong">
										<div class="uer_zhixun_lishiList_hezhi_neirong_list">
										<span>{{item.name}}</span>
										<span>{{moment(item.createTime).format('YYYY-MM-DD HH-MM')}}</span>

										</div>
									</div>
								<!-- </router-link> -->
							</div>

							<!-- <span>查看更多 ></span> -->
						</div>
						<div class="_sXxpqwDa">资讯</div>
					</div>
				</el-col>
			</el-row>
			<el-row style="margin-top: 1px;height: 158px;" >
				<router-link :to="{path:'/product/product_videoSearch'}">
				<div class="user_type_one" @mouseenter="mouseFn('one')" @mouseleave="leaveFn('one')">
					
						<div class="_IskksKxv" v-if="oneValue.data"><div class="_3EmITLRt"></div></div>
						<!-- <div class="leftType" v-if="!oneValue.data">
							<h3>{{oneValue.title}}</h3>
							<p :class="[oneValue.data? 'color':'']">{{oneValue.center}}</p>
						</div>
						<div class="rightType" v-if="oneValue.data">
							<h3>{{oneValue.title}}</h3>
							<p :class="[oneValue.data? 'color':'']">{{oneValue.center}}</p>
						</div> -->
						<div class="type_center" :class="[oneValue.data? 'color':'']">
							{{oneValue.title}}
							<p :class="[oneValue.data? 'color':'']">{{oneValue.center}}</p>
							<svg v-if="oneValue.data" width="49" height="56.354" class="_1A2-UCYe _oWUAZip8"><defs><filter id="brand_svg__a" x="0" y="0" width="49" height="56.354" filterUnits="userSpaceOnUse"><feOffset dy="1"></feOffset><feGaussianBlur stdDeviation="1.5" result="blur"></feGaussianBlur><feFlood flood-color="#bf840f"></feFlood><feComposite operator="in" in2="blur"></feComposite><feComposite in="SourceGraphic"></feComposite></filter></defs><g filter="url(#brand_svg__a)"><path data-name="\u8DEF\u5F84 10850" d="M22.893 41.881l19.993-20a.418.418 0 00.122-.333L41.66 5.616a.848.848 0 00-.772-.772L24.955 3.501a.412.412 0 00-.333.122L4.63 23.616a.424.424 0 000 .6l17.667 17.667a.415.415 0 00.596-.002zm6.487-28.2a2.538 2.538 0 110 3.59 2.543 2.543 0 01-.001-3.588zm15 14.955l-2.093-2.088a.424.424 0 00-.6 0l-19.137 19.1L9.994 33.122a.424.424 0 00-.6 0L7.301 35.21a.424.424 0 000 .6l12.857 12.836 2.093 2.088a.424.424 0 00.6 0l21.532-21.495a.424.424 0 00-.001-.6z" fill="#fff"></path></g></svg>
						</div>
					
				</div></router-link>
				<router-link :to="{path:'/product/product_douyinSearch'}">
				<div class="user_type_two" @mouseenter="mouseFn('two')" @mouseleave="leaveFn('two')">
					
					<div class="_IskksKxv" v-if="twoValue.data"><div class="_3EmITLRt"></div></div>
					<div class="type_center" :class="[twoValue.data? 'color':'']">
						{{twoValue.title}}
						<p :class="[twoValue.data? 'color':'']">{{twoValue.center}}</p>
						<svg v-if="twoValue.data" width="59.909" height="49" viewBox="0 0 59.909 49" class="_1A2-UCYe"><defs><filter id="douyin_svg__a" x="0" y="0" width="59.909" height="49" filterUnits="userSpaceOnUse"><feOffset dy="1"></feOffset><feGaussianBlur stdDeviation="1.5" result="blur"></feGaussianBlur><feFlood flood-color="#12b3ae"></feFlood><feComposite operator="in" in2="blur"></feComposite><feComposite in="SourceGraphic"></feComposite></filter></defs><g filter="url(#douyin_svg__a)"><path data-name="\u8DEF\u5F84 10783" fill="#fff" d="M52.682 11.585l-7.273 4.187V7.136A3.64 3.64 0 0041.773 3.5H8.136A3.64 3.64 0 004.5 7.136v32.727A3.64 3.64 0 008.136 43.5h33.636a3.64 3.64 0 003.636-3.636v-8.636l7.273 4.187a1.818 1.818 0 002.727-1.568V13.159a1.819 1.819 0 00-2.726-1.574zM25.489 17.4a.456.456 0 01-.455.455H12.682a.456.456 0 01-.455-.455v-5.722a.456.456 0 01.455-.455h12.353a.456.456 0 01.455.455zm25.829 12.517l-5.909-3.4v-6.04l5.909-3.4z"></path></g></svg>
					</div>
					<!-- <h3>{{twoValue.title}}</h3>
					<p :class="[twoValue.data? 'color':'']">{{twoValue.center}}</p> -->
				
				</div>
					</router-link>
				<router-link :to="{path:'/product/product_addressSearch'}">
					<div class="user_type_three" @mouseenter="mouseFn('three')" @mouseleave="leaveFn('three')">
					
						<div class="_IskksKxv" v-if="threeValue.data"><div class="_3EmITLRt"></div></div>
						<div class="type_center" :class="[threeValue.data? 'color':'']">
							{{threeValue.title}}
							<p :class="[threeValue.data? 'color':'']">{{threeValue.center}}</p>
							<svg v-if="threeValue.data" width="49" height="56.844" viewBox="0 0 49 56.844" class="_1A2-UCYe"><defs><filter id="hotProduct_svg__a" x="0" y="0" width="49" height="56.844" filterUnits="userSpaceOnUse"><feOffset dy="1"></feOffset><feGaussianBlur stdDeviation="1.5" result="blur"></feGaussianBlur><feFlood flood-color="#42a611"></feFlood><feComposite operator="in" in2="blur"></feComposite><feComposite in="SourceGraphic"></feComposite></filter></defs><g filter="url(#hotProduct_svg__a)"><path data-name="\u8DEF\u5F84 10853" fill="#fff" d="M24.5 17.479a6.021 6.021 0 104.258 1.763 5.978 5.978 0 00-4.258-1.763zm18.419-2.038a19.489 19.489 0 00-4.3-6.22 19.939 19.939 0 00-6.355-4.183 20.258 20.258 0 00-21.892 4.177 19.548 19.548 0 00-4.3 6.22A19.1 19.1 0 004.5 23.07a25.389 25.389 0 002.694 11.22 35.517 35.517 0 005.968 8.5 48.021 48.021 0 0010.129 8.226 2.375 2.375 0 002.409 0 48.019 48.019 0 0010.129-8.226 35.41 35.41 0 005.968-8.5A25.2 25.2 0 0044.5 23.075a19.094 19.094 0 00-1.581-7.634zM24.5 32.962a9.462 9.462 0 119.462-9.462 9.463 9.463 0 01-9.462 9.462z"></path></g></svg>
						</div>
						<!-- <h3>{{threeValue.title}}</h3>
						<p :class="[threeValue.data? 'color':'']">{{threeValue.center}}</p> -->
					
					</div>
				</router-link>
				<router-link :to="{path:'/product/product_user'}">
					<div class="user_type_four" @mouseenter="mouseFn('four')" @mouseleave="leaveFn('four')">
					
						<div class="_IskksKxv" v-if="fourValue.data"><div class="_3EmITLRt"></div></div>
						<div class="type_center" :class="[fourValue.data? 'color':'']">
							{{fourValue.title}}
							<p :class="[fourValue.data? 'color':'']">{{fourValue.center}}</p>
							<svg v-if="fourValue.data" width="49" height="49" viewBox="0 0 49 49" class="_1A2-UCYe"><defs><filter id="brandSearch_svg__a" x="0" y="0" width="49" height="49" filterUnits="userSpaceOnUse"><feOffset dy="1"></feOffset><feGaussianBlur stdDeviation="1.5" result="blur"></feGaussianBlur><feFlood flood-color="#cc6000"></feFlood><feComposite operator="in" in2="blur"></feComposite><feComposite in="SourceGraphic"></feComposite></filter></defs><g filter="url(#brandSearch_svg__a)"><path data-name="\u8DEF\u5F84 10852" fill="#fff" d="M43 11.505V5.1a1.6 1.6 0 00-1.6-1.6H7.6A1.6 1.6 0 006 5.1v6.405A1.6 1.6 0 004.5 13.1v6.585A8.973 8.973 0 006 24.65V41.9a1.6 1.6 0 001.6 1.6h13.7v-8.8h6.4v8.8h13.7a1.6 1.6 0 001.6-1.6V24.65a8.749 8.749 0 00.78-1.445 8.937 8.937 0 00.72-3.52V13.1a1.6 1.6 0 00-1.5-1.595zm-3.6 28.4h-8.5v-6.8a1.6 1.6 0 00-1.6-1.6h-9.6a1.6 1.6 0 00-1.6 1.6v6.8H9.6v-12.11c.145.07.3.14.45.2a9.14 9.14 0 007.04 0 9.142 9.142 0 001.935-1.1.032.032 0 01.03 0 9.131 9.131 0 008.975 1.1 9.142 9.142 0 001.935-1.1.032.032 0 01.03 0 9.131 9.131 0 008.975 1.1c.15-.065.3-.13.45-.2V39.9zm0-28.4H9.6v-4.4h29.8z"></path></g></svg>
						</div>
						<!-- <h3>{{fourValue.title}}</h3>
						<p :class="[fourValue.data? 'color':'']">{{fourValue.center}}</p> -->
					
					</div>
				</router-link>
				<router-link :to="{path:'/product/ruzhu'}">
					<div class="user_type_five" @mouseenter="mouseFn('five')" @mouseleave="leaveFn('five')">
					
						<div class="_IskksKxv" v-if="fiveValue.data"><div class="_3EmITLRt"></div></div>
						<div class="type_center" :class="[fiveValue.data? 'color':'']">
							{{fiveValue.title}}
							<p :class="[fiveValue.data? 'color':'']">{{fiveValue.center}}</p>
							<svg v-if="fiveValue.data" width="49" height="56.354" class="_1A2-UCYe _oWUAZip8"><defs><filter id="brand_svg__a" x="0" y="0" width="49" height="56.354" filterUnits="userSpaceOnUse"><feOffset dy="1"></feOffset><feGaussianBlur stdDeviation="1.5" result="blur"></feGaussianBlur><feFlood flood-color="#bf840f"></feFlood><feComposite operator="in" in2="blur"></feComposite><feComposite in="SourceGraphic"></feComposite></filter></defs><g filter="url(#brand_svg__a)"><path data-name="\u8DEF\u5F84 10850" d="M22.893 41.881l19.993-20a.418.418 0 00.122-.333L41.66 5.616a.848.848 0 00-.772-.772L24.955 3.501a.412.412 0 00-.333.122L4.63 23.616a.424.424 0 000 .6l17.667 17.667a.415.415 0 00.596-.002zm6.487-28.2a2.538 2.538 0 110 3.59 2.543 2.543 0 01-.001-3.588zm15 14.955l-2.093-2.088a.424.424 0 00-.6 0l-19.137 19.1L9.994 33.122a.424.424 0 00-.6 0L7.301 35.21a.424.424 0 000 .6l12.857 12.836 2.093 2.088a.424.424 0 00.6 0l21.532-21.495a.424.424 0 00-.001-.6z" fill="#fff"></path></g></svg>
						</div>
						<!-- <h3>{{fiveValue.title}}</h3>
						<p :class="[fiveValue.data? 'color':'']">{{fiveValue.center}}</p> -->
					
					</div>
				</router-link>
			</el-row>
		</div>
		</div>
	</div>
</template>

<script>
import axios from "axios";
import qs from "qs";
export default {
  name: "gene",
  data() {
    return {
		loading:true,
		login:null,
		oneValue:{title:'素材创意',center:'看集赞最多的视频作品',data:false},
		twoValue:{title:'找视频号',center:'找涨粉最快的视频达人',data:false},
		threeValue:{title:'探店打卡',center:'探寻网红打卡地',data:false},
		fourValue:{title:'商学院',center:'',data:false},
		fiveValue:{title:'博主入驻',center:'',data:false},
		list:[{url:'/article?data=20200421160608957922657665932315',src:require('../../assets/img/videoNew.jpg')}],
		typeList:[],
		articleOne:[],
		articleTwo:[],
		articleThree:[],
		pageOne:1,
		pageTwo:1,
		pageThree:1,
		loadOne:false,
		loadTwo:false,
		loadThree:false,
    };
  },
  activated(){
	  debugger
	  console.log('s')
	 this.login = this.$store.state.login
	   console.log(this.login)
	 
	   if(this.$route.meta.auth && !this.$store.state.login){
	      this.$store.state.loginComponent.getData();
	  }
	 
	  this.$axios
	 .get('my/wx-videoaccount')
	 .then(res => {
	 	if(res.data.code ==0)
	 		this.$store.state.wxVideoaccount=res.data.data
	 })
	this.loading=false;
	this.getDataType();

  },
	mounted() {
		
	},
	methods: {
		mouseFn(_value){
			switch(_value){
				case 'one':
				this.oneValue.title = '3.4亿素材'
				this.oneValue.center = '素材创意'
				this.oneValue.data = true
				break;
				case 'two':
				this.twoValue.title = '8090.3w达人'
				this.twoValue.center = '找视频号'
				this.twoValue.data = true
				break;
				case 'three':
				this.threeValue.title = '48.8w个位置'
				this.threeValue.center = '探店打卡'
				this.threeValue.data = true
				break;
				case 'four':
				this.fourValue.title = '商学院'
				this.fourValue.center = ''
				this.fourValue.data = true
				break;
				case 'five':
				this.fiveValue.title = '博主入驻'
				this.fiveValue.center = ''
				this.fiveValue.data = true
				break;
			}
		},
		leaveFn(_value){
			switch(_value){
				case 'one':
				this.oneValue.title = '素材创意'
				this.oneValue.center = '素材创意'
				this.oneValue.data = false
				break;
				case 'two':
				this.twoValue.title = '找视频号'
				this.twoValue.center = '找涨粉最快的视频达人'
				this.twoValue.data = false
				break;
				case 'three':
				this.threeValue.title = '探店打卡'
				this.threeValue.center = '探寻网红打卡地'
				this.threeValue.data = false
				break;
				case 'four':
				this.fourValue.title = '商学院'
				this.fourValue.center = ''
				this.fourValue.data = false
				break;
				case 'five':
				this.fiveValue.title = '博主入驻'
				this.fiveValue.center = ''
				this.fiveValue.data = false
				break;
			}
		},
    askIfEnter(){
				if(this.$store.state.wxVideoaccount){
			if(this.$store.state.wxVideoaccount.audit==12){
				this.$confirm(this.$store.state.wxVideoaccount.audit12Message+'，是否重新认证?', '提示', {
						confirmButtonText: '确定',
						cancelButtonText: '取消',
						type: 'warning'
					}).then(() => {
					this.$router.push({path:'/product/ruzhu'});
				})
			}else{
			this.$router.push({path:'/product/ruzhu'});
			}
		}else{
			this.$router.push({path:'/product/ruzhu'});
		}
    },
		detailClickFn(_data){
			console.log(_data)
			if(_data.link==0){
				// this.$router.resolve({path: '/articleDetails',query:{data:JSON.stringify(_data)}})
				// window.open('/#/articleDetails?data='+_data.articleId, '_blank');
				window.open('/article.jsp?articleId='+_data.articleId, '_blank');
			}else if (_data.link==1){
				window.open(_data.link1Url, '_blank');
			}
		},
		getDataType(){
			this.loadOne = true;
			this.loadTwo = true;
			this.loadThree = true;
			this.$axios.get("/article-classification/article-classification-list?"+qs.stringify({sort:"orderNo",order:"asc",articleClassificationUpperId:0}))
			.then(res=>{
				if(res.data.codeMsg)
				   this.$message(res.data.codeMsg);
				if(res.data.code == 0){
				   for(let i in res.data.data.itemList){
				   	this.typeList.push(res.data.data.itemList[i])
				   }
				}
				else{
				   //开始失败逻辑
					this.$store.state.loginComponent.getData();
				}
				// this.articleOne = [],
				// this.articleTwo = [],
				// this.articleThree = [],
				// this.pageOne = 1,
				// this.pageTwo = 1,
				// this.pageThree = 1,
				this.nextPageOne();
				this.nextPageTwo();
				this.nextPageThree();
				
				this.loadOne = false;
				this.loadTwo = false;
				this.loadThree = false;
			})
			.catch()
		},
		getDataOne(){
			this.loadOne = true;
			debugger
			 this.$axios.get("/article/article-list?"+qs.stringify({
				articleClassification1Id:this.typeList[0].articleClassificationId,
				pn:this.pageOne,
				ps:5}))
			.then(res=>{
				if(res.data.codeMsg)
				   this.$message(res.data.codeMsg);
				if(res.data.code == 0){
				   for(let i in res.data.data.itemList){
				   	this.articleOne.push(res.data.data.itemList[i])
				   }
				}
				else{
				   //开始失败逻辑
					this.$store.state.loginComponent.getData();

				}
				this.loadOne = false
			})
			.catch()
		},
		getDataTwo(){
			this.loadTwo = true
			debugger
			this.$axios.get("/article/article-list?"+qs.stringify({
				articleClassification1Id:this.typeList[1].articleClassificationId,
				pn:this.pageTwo,
				ps:5}))
			.then(res=>{
				if(res.data.codeMsg)
				   this.$message(res.data.codeMsg);
				if(res.data.code == 0){
				   for(let i in res.data.data.itemList){
				   	this.articleTwo.push(res.data.data.itemList[i])
				   }
				}
				else{
				   //开始失败逻辑
					this.$store.state.loginComponent.getData();
				}
				this.loadTwo = false
			})
			.catch()
		},
		getDataThree(){
			this.$axios.get("/article/article-list?"+qs.stringify({
				articleClassification1Id:this.typeList[2].articleClassificationId,
				pn:this.pageThree,
				ps:5}))
			.then(res=>{
				if(res.data.code == 20){
					this.$store.state.loginComponent.getData();
				}else{
					for(let i in res.data.data.itemList){
						if(i == res.data.data.itemList.length-1){
							this.articleThree.push({
								name:res.data.data.itemList[i].name,
								createTime:res.data.data.itemList[i].createTime,
								data:false,
								link:res.data.data.itemList[i].link,
								articleId:res.data.data.itemList[i].articleId,
								link1Url:res.data.data.itemList[i].link1Url,
							})
						}else{
							this.articleThree.push({
								name:res.data.data.itemList[i].name,
								createTime:res.data.data.itemList[i].createTime,
								data:true,
								link:res.data.data.itemList[i].link,
								articleId:res.data.data.itemList[i].articleId,
								link1Url:res.data.data.itemList[i].link1Url,
							})
						}
						
							// res.data.data.itemList[i])
					}
					this.loadThree = false
				}
			})
			.catch()
		},
		nextPageOne(){
			this.getDataOne()
			this.pageOne++;
		},
		nextPageTwo(){
			this.getDataTwo()
			this.pageTwo++;
		},
		nextPageThree(){
			this.getDataThree()
			this.pageThree++;
		}
	}
};
</script>

<style scoped>
.showPage_eight .el-carousel__button{
    width: 6px !important;
    height: 6px !important;

       padding: 0;
       color: transparent;
       font-size: 0;
       background: #2b2b2b;
       border: 0;
       border-radius: 3px;
       outline: none;
       cursor: pointer;
       opacity: .3;
       -webkit-transition: all .5s;
       transition: all .5s;
  }
.showPage_eight .el-carousel__indicator.is-active button{
      width: 32px !important;
      height: 6px !important;
      border-radius: 3px !important;
      background: #ff7800 !important;
    }
.el-carousel__indicators{
   bottom: 0 !important;
  }
  
a {text-decoration:none; color: rgba(255, 255, 255, 1);}
a:link{text-decoration:none; }
a:hover{text-decoration:none; }
a:active{text-decoration:none; }
a:visited{text-decoration:none; }
div,dl,dt,dd,ul,ol,li,h1,h2,h3,h4,h5,h6,pre,form,fieldset,input,textarea,blockquote,p{
	list-style: none;
}
h1,h2,h3,h4,h5,h6,p{
	font-size: inherit;font-weight: normal;
	margin-block-start: 0rem !important;
	margin-block-end: 0rem !important;
}
.user{
	/* height: 100%; */
	min-width: 1020px;
	/* overflow-x: auto; */
}
.first{

	width: 100%;
}
.user_name{
	height: 300px;
	margin-top: 24px;
	width: 100%;
}
.user_quanxian{
	width: 100%;
	height: 300px;
	background: #3a3a3e;
	position: relative;
}
._1xvNCILN {
    left: 10%;
}
._1aHAtMPw {
    position: absolute;
    width: 4px;
    height: 4px;
    background: #3a3a3e;
    border: 2px solid #2c2a2b;
    border-radius: 50%;
    bottom: -5px;
    right: 10%;
    z-index: 10;
}
.user_quanxian_banben{
	width: 82.4%;
	margin: 0px auto;
	padding-top: 26px;
	padding-bottom: 30px;
}
.user_quanxian_banben_mianfei{
	display: inline;position: relative;
}
.user_quanxian_banben_mianfei>svg{
	position: absolute;
	top:0;
	bottom: 0;
	left: -18px;
	margin: auto 0px;
}
.user_quanxian_banben_shezhi{
	float: right;position: relative;
}
.user_quanxian_banben_shezhi>svg{
	position: absolute;
	top:0;
	bottom: 0;
	left: -17px;
	margin: auto 0px;
}
.user_message{
	text-align: center;
}
.user_message>p:last-child{
	padding-top: 40px;
	font-size: 14px;
}
.user_message>img{
	height: 48px;
	width: 48px;
	border-radius: 50%;
}
.user_message>h5{
	font-weight: 700;
	font-size: 20px;
	padding: 20px 0px 10px;
}
.user_message>p span{
	color: #1890ff;
	cursor: pointer;
}
>>>.el-carousel__indicators {
    display: none!important;
}
.uer_zhixun_gongneng{
	height: 142px;background: #3a3a3e;
	padding: 23px 16px 24px 24px;
}
.uer_zhixun_gongneng_hezi{
	width: 100%;
	height: 100%;
	/* overflow-y: scroll; */
	/* overflow-x: hidden; */
}
.uer_zhixun_gongneng_hezi span{
	width: 100%; padding: 5px;
	box-sizing: bo;
}
.uer_zhixun_gongneng_hezi span,.uer_zhixun_lishi>span{
	height: 19px;
	line-height: 19px;
	white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
	display: block;
	font-size:14px;
}

.uer_zhixun_gongneng_hezi span:hover,.uer_zhixun_tuisongList_hezhi:hover,.uer_zhixun_lishiList_hezhi_neirong_list:hover{
	background: hsla(0,0%,100%,.08);
	color: #fff;
	cursor: pointer;
	transition: all .3s,height 0s;
}
.uer_zhixun_lishiList_hezhi_neirong_list{padding: 5px 5px;}
/* .uer_scroll::-webkit-scrollbar{width:4px;border-radius: 50px;} */
/* .uer_scroll::-webkit-scrollbar-track{background-color:#2b2b2e;border-radius: 50px;} */
/* .uer_scroll::-webkit-scrollbar-thumb{background-color:#66666d;border-radius: 50px;} */
/* .uer_scroll::-webkit-scrollbar-thumb:hover {background-color:#2b2b2e;border-radius: 50px;} */
/* .uer_scroll::-webkit-scrollbar-thumb:active {background-color:#2b2b2e;border-radius: 50px;} */
.uer_zhixun_tuisong,.uer_zhixun_lishi{
	height: 142px;background: #3a3a3e;
	/* width: 100%; */
	padding: 23px 16px 24px 24px;
}
.uer_scroll{
	position: relative;
	/* height: 100%; */
	/* overflow-y: scroll; */
}
.uer_zhixun_tuisongList{
	height: 100%;
	width: 100%;
	/* overflow-y: scroll; */
	overflow-x:hidden
}
.uer_zhixun_tuisongList>span,.uer_zhixun_lishiList>span{
	display:block;
	width: 90px;
	text-align: center;
	margin: 12px auto 0px;
	color: #ff7800;
}
.uer_zhixun_tuisongList_hezhi{
	height: 45px;
	line-height: 25px;
	margin-bottom: 7px;
	padding: 5px;
	/* border-radius: 4px; */
}
.uer_zhixun_tuisongList_hezhi>p:first-child>span{
	font-size: 12px;
	color: #cdcfcf;
	display: inline-block;
	margin-right: 2px;
}
.uer_zhixun_tuisongList_hezhi>p:first-child{
	color: #fff;
}
.uer_zhixun_tuisongList_hezhi>p{
	font-size: 14px;
	color: #787a7a;
	width: 100%;
	padding-right: 20px;
	white-space: nowrap;
	overflow: hidden;
	text-overflow: ellipsis;
}
.uer_zhixun_lishi{
	height: 142px;background: #3a3a3e;
}
.uer_zhixun_lishiList{
	/* position: relative; */
	margin: 0;
	/* padding: 0 0 20px; */
	font-size: 14px;
	list-style: none;
	height: 100%;
	width: 100%;
	/* overflow-y: scroll; */
	overflow-x:hidden;
}
.ant-timeline-item-tail {
    position: absolute;
    top: 25px;
    left: 4px;
    height: calc(100% - 10px);
    border-left: 2px solid #6d6d6d;
}
.ant-timeline-item-head-gray {
    color: #6b6d6d;
    border-color: #6b6d6d!important;
}
.ant-timeline-item-head {
    position: absolute;
	top: 15px;
    width: 6px;
    height: 6px;
    background-color: #2b2b2e;
    border: 2px solid transparent;
    border-radius: 100px;
}
.uer_zhixun_lishiList_hezhi{
	position: relative;
	margin: 0;
	/* padding: 0 0 20px; */
	font-size: 14px;
	list-style: none;
	/* padding-bottom: 16px; */
	height: 60px;

}
.uer_zhixun_lishiList_hezhi_neirong{
	position: relative;
	/* top: -6px; */
	margin: 0 0 0 18px;
	word-break: break-word;
	padding: 5px;
	padding-left: 0px;
}
.uer_zhixun_lishiList_hezhi_neirong span:first-child{
	font-size: 14px;
	display:block;
	margin-bottom: 8px;
	padding-right: 10px;
	color: #fff;
	white-space: nowrap;
	overflow: hidden;
	text-overflow: ellipsis;
}
.uer_zhixun_lishiList_hezhi_neirong span:last-child{
	display:block;
	font-size: 12px;
	color: #787a7a;
}
.user_type_one,.user_type_two,.user_type_three,.user_type_four,.user_type_five{
	box-sizing: border-box;
	height: 100%;
	width: 20%;
	background: rgb(58, 58, 62);
	/* margin-right: 1px; */
	/* display: inline-block; */
	float: left;
	position: relative;
	overflow: hidden;
	text-align: center;
  border-right: 1px solid #2b2b2e;
	/* color: rgb(255, 255, 255); */
}
.type_center{
	width: auto;
	font-weight: 400;
	font-size: 34px;
	display: inline-block;
	margin-top: 40px;
}
.type_center>p{
	width: auto;
	color: rgb(120, 122, 122);
	text-align: left;
	text-align: left;
    padding-top: 15px;
    font-size: 14px;
}
.type_center>svg{
	position: absolute;
	right: 20px;
	bottom: 10px;
}
/* .leftType{
	position: absolute;
	right: 0;
	bottom: 0;
	left: 0;
	top: 0;
	height: 80px;
	width: 145px;
	margin: auto;
	text-align: left;
}
.leftType>h3{
	font-weight: 400;
	font-size: 34px;
	text-aligin:left;
}
.leftType>p{
	bottom: 35px;
	color: rgb(120, 122, 122);
	text-aligin:left;
}
.rightType{

} */
/* .user_type_one h3,.user_type_two h3,.user_type_three h3,.user_type_four h3,.user_type_five h3{
	position: absolute;
	left: 0;
	right: 0;
	top: 48px;
	font-weight: 400;
	font-size: 34px;
}
.user_type_one p,.user_type_two p,.user_type_three p,.user_type_four p,.user_type_five p{
	position: absolute;
	left: 0;
	right: 0;
	bottom: 35px;
	text-align: left;
	color: rgb(120, 122, 122);
} */
.color{
	color: #fff!important;
}
.user_type_one:hover{
	background-color: rgb(24, 144, 255);
	cursor: pointer;
	color: #fff!important;
}
.user_type_two:hover{
	background-color: rgb(254, 44, 85);
	cursor: pointer;
	color: #fff!important;
}
.user_type_three:hover{
	background-color: #52c41a;
	cursor: pointer;
	color: #fff!important;
}
.user_type_four:hover{
	background-color: #ff7800;
	cursor: pointer;
	color: #fff!important;
}
.user_type_five:hover{
	background-color: rgb(250, 173, 20);
	cursor: pointer;
	color: #fff!important;
}
._IskksKxv {
    position: absolute;
    width: 157px;
    height: 157px;
    background: hsla(0,0%,100%,.1);
    border-radius: 50%;
    left: -14%;
    top: -18%;
}
._3EmITLRt {
    width: 131px;
    height: 131px;
    background: #fff;
    border-radius: 50%;
    opacity: .25;
    margin-top: -20px;
    margin-left: -16px;
}
._sXxpqwDa{
	    position: absolute;
	    font-size: 64px;
	    color: #fff;
	    opacity: .04;
	    right: 25px;
	    bottom: 9px;
	    z-index: 0;
		font-family: DINPro Medium,-apple-system,BlinkMacSystemFont,Segoe UI,PingFang SC,Hiragino Sans GB,Microsoft YaHei,Helvetica Neue,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol;
	}
</style>
