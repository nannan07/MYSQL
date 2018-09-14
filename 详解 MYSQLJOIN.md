<div id="img-content">
	<h2 class="rich_media_title" id="activity-name">详解 MYSQL JOIN</h2>
	<div id="meta_content" class="rich_media_meta_list">
		<span class="rich_media_meta rich_media_meta_nickname" id="profileBt">
			<a href="javascript:void(0);" id="js_name"> 数据分析与开发 </a>
			<div id="js_profile_qrcode" class="profile_container"
				style="display: none;">
				<div class="profile_inner">
					<strong class="profile_nickname">数据分析与开发</strong> 
                    <img class="profile_avatar" id="js_profile_qrcode_img" src="" alt="">
					<p class="profile_meta">
						<label class="profile_meta_label">微信号</label> <span
							class="profile_meta_value">DBDevs</span>
					</p> 
					<p class="profile_meta">
						<label class="profile_meta_label">功能介绍</label> <span
							class="profile_meta_value">伯乐在线旗下账号，分享数据分析与开发相关技术文章、教程、工具。</span>
					</p> 
				</div>
				<span class="profile_arrow_wrp" id="js_profile_arrow_wrp"> <i
					class="profile_arrow arrow_out"></i> <i
					class="profile_arrow arrow_in"></i>
				</span>
			</div>
		</span> <em id="publish_time" class="rich_media_meta rich_media_meta_text">8月6日</em>
	</div>
	<div class="rich_media_content " id="js_content">
		<p
			style="white-space: normal; max-width: 100%; min-height: 1em; color: rgb(51, 51, 51); text-align: center;">
			<span
				style="max-width: 100%; font-size: 14px; color: rgb(255, 0, 0); line-height: 25.6px; box-sizing: border-box !important; word-wrap: break-word !important;">（点击</span><span
				style="max-width: 100%; font-size: 14px; line-height: 25.6px; color: rgb(0, 82, 255); box-sizing: border-box !important; word-wrap: break-word !important;">上方蓝字</span><span
				style="max-width: 100%; font-size: 14px; color: rgb(255, 0, 0); line-height: 25.6px; box-sizing: border-box !important; word-wrap: break-word !important;">，快速关注我们）</span>
		</p>
		<p
			style="white-space: normal; max-width: 100%; min-height: 1em; color: rgb(51, 51, 51);">
			<span
				style="max-width: 100%; text-align: center; color: rgb(255, 0, 0); line-height: 25.6px; font-size: 14px; box-sizing: border-box !important; word-wrap: break-word !important;"><br
				style="max-width: 100%; box-sizing: border-box !important; word-wrap: break-word !important;"></span>
		</p>
		<blockquote style="white-space: normal; max-width: 100%;">
			<p
				style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
				<span
					style="max-width: 100%; font-size: 14px; color: rgb(51, 51, 51); box-sizing: border-box !important; word-wrap: break-word !important;">来源：llinvokerl</span>
			</p>
			<p
				style="color: rgb(51, 51, 51); max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
				<span
					style="max-width: 100%; font-size: 14px; box-sizing: border-box !important; word-wrap: break-word !important;">segmentfault.com/a/1190000015572505</span>
			</p>
		</blockquote>
		<p style="white-space: normal;">
			<br
				style="max-width: 100%; box-sizing: border-box !important; word-wrap: break-word !important;">
		</p>
		<h4
			style="margin-bottom: 1rem; font-size: 18px; max-width: 100%; box-sizing: border-box;">
			<span
				style="max-width: 100%; color: rgb(204, 0, 0); box-sizing: border-box !important; word-wrap: break-word !important;"><strong
				style="max-width: 100%; box-sizing: border-box !important; word-wrap: break-word !important;">0
					索引</strong></span>
		</h4>
		<ul class="list-paddingleft-2" style="list-style-type: square;">
			<li><p
					style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
					<span
						style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); line-height: 22px; word-wrap: break-word !important; font-size: 14px !important;"><strong
						style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">JOIN</strong>语句的执行顺序</span>
				</p></li>
			<li><p
					style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
					<span
						style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); line-height: 22px; word-wrap: break-word !important; font-size: 14px !important;"><strong
						style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">INNER/LEFT/RIGHT/FULL
							JOIN</strong>的区别</span>
				</p></li>
			<li><p
					style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
					<span
						style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); line-height: 22px; word-wrap: break-word !important; font-size: 14px !important;"><strong
						style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">ON</strong>和<strong
						style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">WHERE</strong>的区别</span>
				</p></li>
		</ul>
		<h4
			style="margin-top: 1.5rem; margin-bottom: 1rem; font-size: 18px; max-width: 100%; box-sizing: border-box;">
			<span
				style="max-width: 100%; color: rgb(204, 0, 0); box-sizing: border-box !important; word-wrap: break-word !important;"><strong
				style="max-width: 100%; box-sizing: border-box !important; word-wrap: break-word !important;">1
					概述</strong></span>
		</h4>
		<p
			style="margin-top: 15px; margin-bottom: 15px; max-width: 100%; box-sizing: border-box; min-height: 1em; letter-spacing: 0.544px; text-align: justify; background-color: rgb(255, 255, 255); font-size: 16px; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">一个完整的SQL语句中会被拆分成多个子句，子句的执行过程中会产生虚拟表(vt)，但是结果只返回最后一张虚拟表。从这个思路出发，我们试着理解一下JOIN查询的执行过程并解答一些常见的问题。</p>
		<p
			style="margin-top: 15px; margin-bottom: 15px; max-width: 100%; box-sizing: border-box; min-height: 1em; letter-spacing: 0.544px; text-align: justify; background-color: rgb(255, 255, 255); font-size: 16px; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">
			如果之前对不同JOIN的执行结果没有概念，可以结合这篇文章： <span
				style="max-width: 100%; color: rgb(30, 107, 184); box-sizing: border-box !important; word-wrap: break-word !important;">https://www.codeproject.com/Articles/33052/Visual-Representation-of-SQL-Joins</span>往下看。
		</p>
		<h4
			style="margin-top: 1.5rem; margin-bottom: 1rem; font-size: 18px; max-width: 100%; box-sizing: border-box;">
			<span
				style="max-width: 100%; color: rgb(204, 0, 0); box-sizing: border-box !important; word-wrap: break-word !important;"><strong
				style="max-width: 100%; box-sizing: border-box !important; word-wrap: break-word !important;">2
					JOIN的执行顺序</strong></span>
		</h4>
		<p
			style="margin-top: 15px; margin-bottom: 15px; max-width: 100%; box-sizing: border-box; min-height: 1em; letter-spacing: 0.544px; text-align: justify; background-color: rgb(255, 255, 255); font-size: 16px; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">以下是JOIN查询的通用结构：</p>
		<pre class=""
			style="margin-top: 0px; margin-bottom: 0px; padding: 8px 0px 6px; max-width: 100%; box-sizing: border-box; letter-spacing: 0.544px; text-align: justify; background-color: rgb(47, 54, 64); border-radius: 0px; overflow-y: auto; color: rgb(80, 97, 109); font-size: 10px; line-height: 12px; word-wrap: break-word !important;">
			<ol class="list-paddingleft-2" style="list-style-type: none;">
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">SELECT </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(255, 206, 84); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">&lt;row_list&gt;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> </span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> &nbsp;FROM </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(255, 206, 84); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">&lt;left_table&gt;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> </span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> &nbsp; &nbsp;&lt;inner|left|right&gt; JOIN </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(255, 206, 84); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">&lt;right_table&gt;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> </span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> &nbsp; &nbsp; &nbsp;ON &lt;join condition&gt; </span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> &nbsp; &nbsp; &nbsp; &nbsp;WHERE </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(255, 206, 84); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">&lt;where_condition&gt;</span>
							</code></span>
					</p></li>
			</ol>
		</pre>
		<p
			style="margin-top: 15px; margin-bottom: 15px; max-width: 100%; box-sizing: border-box; min-height: 1em; letter-spacing: 0.544px; text-align: justify; background-color: rgb(255, 255, 255); font-size: 16px; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">
			它的执行顺序如下<strong
				style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">(SQL语句里第一个被执行的总是FROM子句)</strong>：
		</p>
		<ul class="list-paddingleft-2" style="list-style-type: square;">
			<li><p
					style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
					<span
						style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); line-height: 22px; word-wrap: break-word !important; font-size: 14px !important;"><strong
						style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">FROM</strong>:对左右两张表执行笛卡尔积，产生第一张表vt1。行数为n*m（n为左表的行数，m为右表的行数</span>
				</p></li>
			<li><p
					style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
					<span
						style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); line-height: 22px; word-wrap: break-word !important; font-size: 14px !important;"><strong
						style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">ON</strong>:根据ON的条件逐行筛选vt1，将结果插入vt2中</span>
				</p></li>
			<li><p
					style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
					<span
						style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); line-height: 22px; word-wrap: break-word !important; font-size: 14px !important;"><strong
						style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">JOIN</strong>:添加外部行，如果指定了<strong
						style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;"><span
							style="max-width: 100%; box-sizing: border-box; font-weight: 400; word-wrap: break-word !important;">LEFT
								JOIN</span></strong>(<strong
						style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;"><span
							style="max-width: 100%; box-sizing: border-box; font-weight: 400; word-wrap: break-word !important;">LEFT
								OUTER JOIN</span></strong>)，则先遍历一遍<strong
						style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">左表</strong>的每一行，其中不在vt2的行会被插入到vt2，该行的剩余字段将被填充为<strong
						style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;"><span
							style="max-width: 100%; box-sizing: border-box; font-weight: 400; word-wrap: break-word !important;">NULL</span></strong>，形成vt3；如果指定了<strong
						style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;"><span
							style="max-width: 100%; box-sizing: border-box; font-weight: 400; word-wrap: break-word !important;">RIGHT
								JOIN</span></strong>也是同理。但如果指定的是<strong
						style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;"><span
							style="max-width: 100%; box-sizing: border-box; font-weight: 400; word-wrap: break-word !important;">INNER
								JOIN</span></strong>，则不会添加外部行，上述插入过程被忽略，vt2=vt3（所以<strong
						style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;"><span
							style="max-width: 100%; box-sizing: border-box; font-weight: 400; word-wrap: break-word !important;">INNER
								JOIN</span></strong>的过滤条件放在<strong
						style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;"><span
							style="max-width: 100%; box-sizing: border-box; font-weight: 400; word-wrap: break-word !important;">ON</span></strong>或<strong
						style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;"><span
							style="max-width: 100%; box-sizing: border-box; font-weight: 400; word-wrap: break-word !important;">WHERE</span></strong>里
						执行结果是没有区别的，下文会细说）</span>
				</p></li>
			<li><p
					style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
					<span
						style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); line-height: 22px; word-wrap: break-word !important; font-size: 14px !important;"><strong
						style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">WHERE</strong>:对vt3进行条件过滤，满足条件的行被输出到vt4</span>
				</p></li>
			<li><p
					style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
					<span
						style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); line-height: 22px; word-wrap: break-word !important; font-size: 14px !important;"><strong
						style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">SELECT</strong>:取出vt4的指定字段到vt5</span>
				</p></li>
		</ul>
		<p
			style="margin-top: 15px; margin-bottom: 15px; max-width: 100%; box-sizing: border-box; min-height: 1em; letter-spacing: 0.544px; text-align: justify; background-color: rgb(255, 255, 255); font-size: 16px; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">下面用一个例子介绍一下上述联表的过程（这个例子不是个好的实践，只是为了说明join语法）。</p>
		<h4
			style="margin-top: 1.5rem; margin-bottom: 1rem; font-size: 18px; max-width: 100%; box-sizing: border-box;">
			<span
				style="max-width: 100%; color: rgb(204, 0, 0); box-sizing: border-box !important; word-wrap: break-word !important;"><strong
				style="max-width: 100%; box-sizing: border-box !important; word-wrap: break-word !important;">3
					举例</strong></span>
		</h4>
		<p
			style="margin-top: 15px; margin-bottom: 15px; max-width: 100%; box-sizing: border-box; min-height: 1em; letter-spacing: 0.544px; text-align: justify; background-color: rgb(255, 255, 255); font-size: 16px; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">创建一个用户信息表：</p>
		<pre class=""
			style="margin-top: 0px; margin-bottom: 0px; padding: 8px 0px 6px; max-width: 100%; box-sizing: border-box; letter-spacing: 0.544px; text-align: justify; background-color: rgb(47, 54, 64); border-radius: 0px; overflow-y: auto; color: rgb(80, 97, 109); font-size: 10px; line-height: 12px; word-wrap: break-word !important;">
			<ol class="list-paddingleft-2" style="list-style-type: none;">
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">CREATE TABLE </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(255, 206, 84); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">`user_info`</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> (</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(255, 206, 84); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">`userid`</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">int</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">(</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">11</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">) NOT NULL,</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(255, 206, 84); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">`name`</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> varchar(</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">255</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">) NOT NULL,</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> &nbsp;UNIQUE </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(255, 206, 84); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">`userid`</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> (</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(255, 206, 84); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">`userid`</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">)</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">) ENGINE=</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">InnoDB</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> DEFAULT CHARSET=utf8mb4</span>
							</code></span>
					</p></li>
			</ol>
		</pre>
		<p
			style="margin-top: 15px; margin-bottom: 15px; max-width: 100%; box-sizing: border-box; min-height: 1em; letter-spacing: 0.544px; text-align: justify; background-color: rgb(255, 255, 255); font-size: 16px; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">再创建一个用户余额表：</p>
		<pre class=""
			style="margin-top: 0px; margin-bottom: 0px; padding: 8px 0px 6px; max-width: 100%; box-sizing: border-box; letter-spacing: 0.544px; text-align: justify; background-color: rgb(47, 54, 64); border-radius: 0px; overflow-y: auto; color: rgb(80, 97, 109); font-size: 10px; line-height: 12px; word-wrap: break-word !important;">
			<ol class="list-paddingleft-2" style="list-style-type: none;">
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">CREATE TABLE </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(255, 206, 84); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">`user_account`</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> (</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(255, 206, 84); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">`userid`</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">int</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">(</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">11</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">) NOT NULL,</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(255, 206, 84); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">`money`</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> bigint(</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">20</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">) NOT NULL,</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> UNIQUE </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(255, 206, 84); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">`userid`</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> (</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(255, 206, 84); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">`userid`</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">)</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">) ENGINE=</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">InnoDB</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> DEFAULT CHARSET=utf8mb4</span>
							</code></span>
					</p></li>
			</ol>
		</pre>
		<p
			style="margin-top: 15px; margin-bottom: 15px; max-width: 100%; box-sizing: border-box; min-height: 1em; letter-spacing: 0.544px; text-align: justify; background-color: rgb(255, 255, 255); font-size: 16px; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">随便导入一些数据：</p>
		<pre class=""
			style="margin-top: 0px; margin-bottom: 0px; padding: 8px 0px 6px; max-width: 100%; box-sizing: border-box; letter-spacing: 0.544px; text-align: justify; background-color: rgb(47, 54, 64); border-radius: 0px; overflow-y: auto; color: rgb(80, 97, 109); font-size: 10px; line-height: 12px; word-wrap: break-word !important;">
			<ol class="list-paddingleft-2" style="list-style-type: none;">
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">select</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> * </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">from</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> user_info;</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| userid | name |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1001</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | x &nbsp; &nbsp;|</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1002</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | y &nbsp; &nbsp;|</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | z &nbsp; &nbsp;|</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1004</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | a &nbsp; &nbsp;|</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1005</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | b &nbsp; &nbsp;|</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1006</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | c &nbsp; &nbsp;|</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1007</span><span
									class="" style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | d &nbsp; &nbsp;|</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1008</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | e &nbsp; &nbsp;|</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">8</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> rows </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">in</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">set</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> (</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">0.00</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> sec)</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;"></code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">select</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> * </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">from</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> user_account;</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| userid | money |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1001</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">22</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1002</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">30</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">8</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1009</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">11</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">4</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> rows </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">in</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">set</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> (</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">0.00</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> sec)</span>
							</code></span>
					</p></li>
			</ol>
		</pre>
		<p
			style="margin-top: 15px; margin-bottom: 15px; max-width: 100%; box-sizing: border-box; min-height: 1em; letter-spacing: 0.544px; text-align: justify; background-color: rgb(255, 255, 255); font-size: 16px; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">一共8个用户有用户名，4个用户的账户有余额。</p>
		<p
			style="margin-top: 15px; margin-bottom: 15px; max-width: 100%; box-sizing: border-box; min-height: 1em; letter-spacing: 0.544px; text-align: justify; background-color: rgb(255, 255, 255); font-size: 16px; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">
			<strong
				style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">取出userid为1003的用户姓名和余额，SQL如下</strong>：
		</p>
		<pre class=""
			style="margin-top: 0px; margin-bottom: 0px; padding: 8px 0px 6px; max-width: 100%; box-sizing: border-box; letter-spacing: 0.544px; text-align: justify; background-color: rgb(47, 54, 64); border-radius: 0px; overflow-y: auto; color: rgb(80, 97, 109); font-size: 10px; line-height: 12px; word-wrap: break-word !important;">
			<ol class="list-paddingleft-2" style="list-style-type: none;">
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">SELECT i.name, a.money </span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> &nbsp;FROM user_info </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">as</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> i </span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> &nbsp; &nbsp;LEFT JOIN user_account </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">as</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> a </span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> &nbsp; &nbsp; &nbsp;ON i.userid = a.userid </span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> &nbsp; &nbsp; &nbsp; &nbsp;WHERE a.userid = </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">;</span>
							</code></span>
					</p></li>
			</ol>
		</pre>
		<h5
			style="margin-top: 1.5rem; margin-bottom: 1rem; max-width: 100%; box-sizing: border-box;">
			<strong
				style="max-width: 100%; box-sizing: border-box !important; word-wrap: break-word !important;">第一步：执行FROM子句对两张表进行笛卡尔积操作</strong>
		</h5>
		<p
			style="margin-top: 15px; margin-bottom: 15px; max-width: 100%; box-sizing: border-box; min-height: 1em; letter-spacing: 0.544px; text-align: justify; background-color: rgb(255, 255, 255); font-size: 16px; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">
			笛卡尔积操作后会返回两张表中所有行的组合，左表user<span
				style="max-width: 100%; box-sizing: border-box; word-wrap: break-word !important;">info有8行，右表user</span>account有4行，生成的虚拟表vt1就是8*4=32行：
		</p>
		<pre class=""
			style="margin-top: 0px; margin-bottom: 0px; padding: 8px 0px 6px; max-width: 100%; box-sizing: border-box; letter-spacing: 0.544px; text-align: justify; background-color: rgb(47, 54, 64); border-radius: 0px; overflow-y: auto; color: rgb(80, 97, 109); font-size: 10px; line-height: 12px; word-wrap: break-word !important;">
			<ol class="list-paddingleft-2" style="list-style-type: none;">
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">SELECT * FROM user_info </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">as</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> i LEFT JOIN user_account </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">as</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> a ON </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">;</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| userid | name | userid | money |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1001</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | x &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1001</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">22</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1002</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | y &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1001</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">22</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | z &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1001</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">22</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1004</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | a &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1001</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">22</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1005</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | b &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1001</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">22</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1006</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | c &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1001</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">22</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1007</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | d &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1001</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">22</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1008</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | e &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1001</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">22</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1001</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | x &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1002</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">30</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1002</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | y &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1002</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">30</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | z &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1002</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">30</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1004</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | a &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1002</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">30</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1005</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | b &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1002</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">30</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1006</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | c &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1002</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">30</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1007</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | d &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1002</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">30</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1008</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | e &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1002</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">30</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1001</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | x &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">8</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1002</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | y &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">8</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | z &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">8</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1004</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | a &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">8</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1005</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | b &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">8</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1006</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | c &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">8</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1007</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | d &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">8</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1008</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | e &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">8</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1001</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | x &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1009</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">11</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1002</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | y &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1009</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">11</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | z &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1009</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">11</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1004</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | a &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1009</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">11</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1005</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | b &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1009</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">11</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1006</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | c &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1009</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">11</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1007</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | d &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1009</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">11</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1008</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | e &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1009</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">11</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">32</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> rows </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">in</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">set</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> (</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">0.00</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> sec)</span>
							</code></span>
					</p></li>
			</ol>
		</pre>
		<h5
			style="margin-top: 1.5rem; margin-bottom: 1rem; max-width: 100%; box-sizing: border-box;">
			<strong
				style="max-width: 100%; box-sizing: border-box !important; word-wrap: break-word !important;">第二步：执行ON子句过滤掉不满足条件的行</strong>
		</h5>
		<p
			style="margin-top: 15px; margin-bottom: 15px; max-width: 100%; box-sizing: border-box; min-height: 1em; letter-spacing: 0.544px; text-align: justify; background-color: rgb(255, 255, 255); font-size: 16px; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">ON
			i.userid = a.userid 过滤之后vt2如下：</p>
		<pre class=""
			style="margin-top: 0px; margin-bottom: 0px; padding: 8px 0px 6px; max-width: 100%; box-sizing: border-box; letter-spacing: 0.544px; text-align: justify; background-color: rgb(47, 54, 64); border-radius: 0px; overflow-y: auto; color: rgb(80, 97, 109); font-size: 10px; line-height: 12px; word-wrap: break-word !important;">
			<ol class="list-paddingleft-2" style="list-style-type: none;">
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| userid | name | userid | money |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1001</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | x &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1001</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">22</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1002</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | y &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1002</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">30</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | z &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">8</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
			</ol>
		</pre>
		<h5
			style="margin-top: 1.5rem; margin-bottom: 1rem; max-width: 100%; box-sizing: border-box;">
			<strong
				style="max-width: 100%; box-sizing: border-box !important; word-wrap: break-word !important;">第三步：JOIN
				添加外部行</strong>
		</h5>
		<p
			style="margin-top: 15px; margin-bottom: 15px; max-width: 100%; box-sizing: border-box; min-height: 1em; letter-spacing: 0.544px; text-align: justify; background-color: rgb(255, 255, 255); font-size: 16px; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">
			<strong
				style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">LEFT
				JOIN</strong>会将左表未出现在vt2的行插入进vt2，每一行的剩余字段将被填充为NULL，<strong
				style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">RIGHT
				JOIN</strong>同理。
		</p>
		<p
			style="margin-top: 15px; margin-bottom: 15px; max-width: 100%; box-sizing: border-box; min-height: 1em; letter-spacing: 0.544px; text-align: justify; background-color: rgb(255, 255, 255); font-size: 16px; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">
			本例中用的是<strong
				style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">LEFT
				JOIN</strong>，所以会将左表<strong
				style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">user_info</strong>剩下的行都添上
			生成表vt3：
		</p>
		<pre class=""
			style="margin-top: 0px; margin-bottom: 0px; padding: 8px 0px 6px; max-width: 100%; box-sizing: border-box; letter-spacing: 0.544px; text-align: justify; background-color: rgb(47, 54, 64); border-radius: 0px; overflow-y: auto; color: rgb(80, 97, 109); font-size: 10px; line-height: 12px; word-wrap: break-word !important;">
			<ol class="list-paddingleft-2" style="list-style-type: none;">
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| userid | name | userid | money |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1001</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | x &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1001</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">22</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1002</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | y &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1002</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">30</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | z &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">8</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1004</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | a &nbsp; &nbsp;| &nbsp; NULL | &nbsp;NULL |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1005</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | b &nbsp; &nbsp;| &nbsp; NULL | &nbsp;NULL |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1006</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | c &nbsp; &nbsp;| &nbsp; NULL | &nbsp;NULL |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1007</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | d &nbsp; &nbsp;| &nbsp; NULL | &nbsp;NULL |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1008</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | e &nbsp; &nbsp;| &nbsp; NULL | &nbsp;NULL |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
			</ol>
		</pre>
		<h5
			style="margin-top: 1.5rem; margin-bottom: 1rem; max-width: 100%; box-sizing: border-box;">
			<strong
				style="max-width: 100%; box-sizing: border-box !important; word-wrap: break-word !important;">第四步：WHERE条件过滤</strong>
		</h5>
		<p
			style="margin-top: 15px; margin-bottom: 15px; max-width: 100%; box-sizing: border-box; min-height: 1em; letter-spacing: 0.544px; text-align: justify; background-color: rgb(255, 255, 255); font-size: 16px; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">WHERE
			a.userid = 1003 生成表vt4：</p>
		<pre class=""
			style="margin-top: 0px; margin-bottom: 0px; padding: 8px 0px 6px; max-width: 100%; box-sizing: border-box; letter-spacing: 0.544px; text-align: justify; background-color: rgb(47, 54, 64); border-radius: 0px; overflow-y: auto; color: rgb(80, 97, 109); font-size: 10px; line-height: 12px; word-wrap: break-word !important;">
			<ol class="list-paddingleft-2" style="list-style-type: none;">
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| userid | name | userid | money |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | z &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">8</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
			</ol>
		</pre>
		<h5
			style="margin-top: 1.5rem; margin-bottom: 1rem; max-width: 100%; box-sizing: border-box;">
			<strong
				style="max-width: 100%; box-sizing: border-box !important; word-wrap: break-word !important;">第五步：SELECT</strong>
		</h5>
		<p
			style="margin-top: 15px; margin-bottom: 15px; max-width: 100%; box-sizing: border-box; min-height: 1em; letter-spacing: 0.544px; text-align: justify; background-color: rgb(255, 255, 255); font-size: 16px; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">SELECT
			i.name, a.money 生成vt5：</p>
		<pre class=""
			style="margin-top: 0px; margin-bottom: 0px; padding: 8px 0px 6px; max-width: 100%; box-sizing: border-box; letter-spacing: 0.544px; text-align: justify; background-color: rgb(47, 54, 64); border-radius: 0px; overflow-y: auto; color: rgb(80, 97, 109); font-size: 10px; line-height: 12px; word-wrap: break-word !important;">
			<ol class="list-paddingleft-2" style="list-style-type: none;">
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| name | money |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| z &nbsp; &nbsp;| &nbsp; &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">8</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+------+-------+</span>
							</code></span>
					</p></li>
			</ol>
		</pre>
		<p
			style="margin-top: 15px; margin-bottom: 15px; max-width: 100%; box-sizing: border-box; min-height: 1em; letter-spacing: 0.544px; text-align: justify; background-color: rgb(255, 255, 255); font-size: 16px; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">虚拟表vt5作为最终结果返回给客户端。</p>
		<p
			style="margin-top: 15px; margin-bottom: 15px; max-width: 100%; box-sizing: border-box; min-height: 1em; letter-spacing: 0.544px; text-align: justify; background-color: rgb(255, 255, 255); font-size: 16px; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">
			介绍完联表的过程之后，我们看看常用<strong
				style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">JOIN</strong>的区别。
		</p>
		<h4
			style="margin-top: 1.5rem; margin-bottom: 1rem; font-size: 18px; max-width: 100%; box-sizing: border-box;">
			<span
				style="max-width: 100%; color: rgb(204, 0, 0); box-sizing: border-box !important; word-wrap: break-word !important;"><strong
				style="max-width: 100%; box-sizing: border-box !important; word-wrap: break-word !important;">4
					INNER/LEFT/RIGHT/FULL JOIN的区别</strong></span>
		</h4>
		<ul class="list-paddingleft-2" style="list-style-type: square;">
			<li><p
					style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
					<span
						style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); line-height: 22px; word-wrap: break-word !important; font-size: 14px !important;"><strong
						style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">INNER
							JOIN...ON...</strong>: 返回 左右表互相匹配的所有行（因为只执行上文的第二步ON过滤，不执行第三步 添加外部行）</span>
				</p></li>
			<li><p
					style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
					<span
						style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); line-height: 22px; word-wrap: break-word !important; font-size: 14px !important;"><strong
						style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">LEFT
							JOIN...ON...</strong>: 返回左表的所有行，若某些行在右表里没有相对应的匹配行，则将右表的列在新表中置为NULL</span>
				</p></li>
			<li><p
					style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
					<span
						style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); line-height: 22px; word-wrap: break-word !important; font-size: 14px !important;"><strong
						style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">RIGHT
							JOIN...ON...</strong>: 返回右表的所有行，若某些行在左表里没有相对应的匹配行，则将左表的列在新表中置为NULL</span>
				</p></li>
		</ul>
		<h5
			style="margin-top: 1.5rem; margin-bottom: 1rem; max-width: 100%; box-sizing: border-box;">
			<strong
				style="max-width: 100%; box-sizing: border-box !important; word-wrap: break-word !important;">INNER
				JOIN</strong>
		</h5>
		<p
			style="margin-top: 15px; margin-bottom: 15px; max-width: 100%; box-sizing: border-box; min-height: 1em; letter-spacing: 0.544px; text-align: justify; background-color: rgb(255, 255, 255); font-size: 16px; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">
			拿上文的第三步<strong
				style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">添加外部行</strong>来举例，若<strong
				style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">LEFT
				JOIN</strong>替换成<strong
				style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">INNER
				JOIN</strong>，则会跳过这一步，生成的表vt3与vt2一模一样：
		</p>
		<pre class=""
			style="margin-top: 0px; margin-bottom: 0px; padding: 8px 0px 6px; max-width: 100%; box-sizing: border-box; letter-spacing: 0.544px; text-align: justify; background-color: rgb(47, 54, 64); border-radius: 0px; overflow-y: auto; color: rgb(80, 97, 109); font-size: 10px; line-height: 12px; word-wrap: break-word !important;">
			<ol class="list-paddingleft-2" style="list-style-type: none;">
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| userid | name | userid | money |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1001</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | x &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1001</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">22</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1002</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | y &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1002</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">30</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | z &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">8</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
			</ol>
		</pre>
		<h5
			style="margin-top: 1.5rem; margin-bottom: 1rem; max-width: 100%; box-sizing: border-box;">
			<strong
				style="max-width: 100%; box-sizing: border-box !important; word-wrap: break-word !important;">RIGHT
				JOIN</strong>
		</h5>
		<p
			style="margin-top: 15px; margin-bottom: 15px; max-width: 100%; box-sizing: border-box; min-height: 1em; letter-spacing: 0.544px; text-align: justify; background-color: rgb(255, 255, 255); font-size: 16px; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">
			若<strong
				style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">LEFT
				JOIN</strong>替换成<strong
				style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">RIGHT
				JOIN</strong>，则生成的表vt3如下：
		</p>
		<pre class=""
			style="margin-top: 0px; margin-bottom: 0px; padding: 8px 0px 6px; max-width: 100%; box-sizing: border-box; letter-spacing: 0.544px; text-align: justify; background-color: rgb(47, 54, 64); border-radius: 0px; overflow-y: auto; color: rgb(80, 97, 109); font-size: 10px; line-height: 12px; word-wrap: break-word !important;">
			<ol class="list-paddingleft-2" style="list-style-type: none;">
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| userid | name | userid | money |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1001</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | x &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1001</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">22</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1002</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | y &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1002</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">30</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | z &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">8</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; NULL | NULL | &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1009</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">11</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
			</ol>
		</pre>
		<p
			style="margin-top: 15px; margin-bottom: 15px; max-width: 100%; box-sizing: border-box; min-height: 1em; letter-spacing: 0.544px; text-align: justify; background-color: rgb(255, 255, 255); font-size: 16px; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">
			<strong
				style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">因为user<span
				style="max-width: 100%; box-sizing: border-box; font-weight: 400; word-wrap: break-word !important;">account（右表）里存在userid=1009这一行，而user</span>info（左表）里却找不到这一行的记录，所以会在第三步插入以下一行：
			</strong>
		</p>
		<pre class=""
			style="margin-top: 0px; margin-bottom: 0px; padding: 8px 0px 6px; max-width: 100%; box-sizing: border-box; letter-spacing: 0.544px; text-align: justify; background-color: rgb(47, 54, 64); border-radius: 0px; overflow-y: auto; color: rgb(80, 97, 109); font-size: 10px; line-height: 12px; word-wrap: break-word !important;">
			<ol class="list-paddingleft-2" style="list-style-type: none;">
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; NULL | NULL | &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1009</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">11</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
			</ol>
		</pre>
		<h5
			style="margin-top: 1.5rem; margin-bottom: 1rem; max-width: 100%; box-sizing: border-box;">
			<strong
				style="max-width: 100%; box-sizing: border-box !important; word-wrap: break-word !important;">FULL
				JOIN</strong>
		</h5>
		<p
			style="margin-top: 15px; margin-bottom: 15px; max-width: 100%; box-sizing: border-box; min-height: 1em; letter-spacing: 0.544px; text-align: justify; background-color: rgb(255, 255, 255); font-size: 16px; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">
			上文引用的文章中提到了标准SQL定义的<strong
				style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">FULL
				JOIN</strong>，这在mysql里是不支持的，不过我们可以通过<strong
				style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">LEFT
				JOIN + UNION + RIGHT JOIN</strong> 来实现<strong
				style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">FULL
				JOIN</strong>：
		</p>
		<pre class=""
			style="margin-top: 0px; margin-bottom: 0px; padding: 8px 0px 6px; max-width: 100%; box-sizing: border-box; letter-spacing: 0.544px; text-align: justify; background-color: rgb(47, 54, 64); border-radius: 0px; overflow-y: auto; color: rgb(80, 97, 109); font-size: 10px; line-height: 12px; word-wrap: break-word !important;">
			<ol class="list-paddingleft-2" style="list-style-type: none;">
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">SELECT * </span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> &nbsp;FROM user_info </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">as</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> i </span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> &nbsp; &nbsp;RIGHT JOIN user_account </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">as</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> a </span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> &nbsp; &nbsp; &nbsp;ON a.userid=i.userid</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">union</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> </span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">SELECT * </span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> &nbsp;FROM user_info </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">as</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> i </span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> &nbsp; &nbsp;LEFT JOIN user_account </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">as</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> a </span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> &nbsp; &nbsp; &nbsp;ON a.userid=i.userid;</span>
							</code></span>
					</p></li>
			</ol>
		</pre>
		<p
			style="margin-top: 15px; margin-bottom: 15px; max-width: 100%; box-sizing: border-box; min-height: 1em; letter-spacing: 0.544px; text-align: justify; background-color: rgb(255, 255, 255); font-size: 16px; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">他会返回如下结果：</p>
		<pre class=""
			style="margin-top: 0px; margin-bottom: 0px; padding: 8px 0px 6px; max-width: 100%; box-sizing: border-box; letter-spacing: 0.544px; text-align: justify; background-color: rgb(47, 54, 64); border-radius: 0px; overflow-y: auto; color: rgb(80, 97, 109); font-size: 10px; line-height: 12px; word-wrap: break-word !important;">
			<ol class="list-paddingleft-2" style="list-style-type: none;">
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| userid | name | userid | money |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1001</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | x &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1001</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">22</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1002</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | y &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1002</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">30</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | z &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">8</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; NULL | NULL | &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1009</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">11</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1004</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | a &nbsp; &nbsp;| &nbsp; NULL | &nbsp;NULL |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1005</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | b &nbsp; &nbsp;| &nbsp; NULL | &nbsp;NULL |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1006</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | c &nbsp; &nbsp;| &nbsp; NULL | &nbsp;NULL |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1007</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | d &nbsp; &nbsp;| &nbsp; NULL | &nbsp;NULL |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1008</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | e &nbsp; &nbsp;| &nbsp; NULL | &nbsp;NULL |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
			</ol>
		</pre>
		<p
			style="margin-top: 15px; margin-bottom: 15px; max-width: 100%; box-sizing: border-box; min-height: 1em; letter-spacing: 0.544px; text-align: justify; background-color: rgb(255, 255, 255); font-size: 16px; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">
			ps：其实我们从语义上就能看出<strong
				style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">LEFT
				JOIN</strong>和<strong
				style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">RIGHT
				JOIN</strong>没什么差别，两者的结果差异取决于左右表的放置顺序，以下内容摘自mysql官方文档：
		</p>
		<blockquote
			style="margin-top: 1em; margin-bottom: 1.2em; padding: 15px 15px 15px 1rem; max-width: 100%; box-sizing: border-box; border-left-width: 6px; border-left-color: rgb(220, 230, 240); letter-spacing: 0.544px; text-align: justify; white-space: normal; color: rgb(129, 145, 152); font-size: 14px; line-height: 22px; background: rgb(242, 247, 251); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">
			<p
				style="max-width: 100%; box-sizing: border-box; min-height: 1em; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); word-wrap: break-word !important;">RIGHT
				JOIN works analogously to LEFT JOIN. To keep code portable across
				databases, it is recommended that you use LEFT JOIN instead of RIGHT
				JOIN.</p>
		</blockquote>
		<p
			style="margin-top: 15px; margin-bottom: 15px; max-width: 100%; box-sizing: border-box; min-height: 1em; letter-spacing: 0.544px; text-align: justify; background-color: rgb(255, 255, 255); font-size: 16px; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">所以当你纠结使用LEFT
			JOIN还是RIGHT JOIN时，尽可能只使用LEFT JOIN吧。</p>
		<h4
			style="margin-top: 1.5rem; margin-bottom: 1rem; font-size: 18px; max-width: 100%; box-sizing: border-box;">
			<span
				style="max-width: 100%; color: rgb(204, 0, 0); box-sizing: border-box !important; word-wrap: break-word !important;"><strong
				style="max-width: 100%; box-sizing: border-box !important; word-wrap: break-word !important;">5
					ON和WHERE的区别</strong></span>
		</h4>
		<p
			style="margin-top: 15px; margin-bottom: 15px; max-width: 100%; box-sizing: border-box; min-height: 1em; letter-spacing: 0.544px; text-align: justify; background-color: rgb(255, 255, 255); font-size: 16px; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">上文把JOIN的执行顺序了解清楚之后，ON和WHERE的区别也就很好理解了。</p>
		<p
			style="margin-top: 15px; margin-bottom: 15px; max-width: 100%; box-sizing: border-box; min-height: 1em; letter-spacing: 0.544px; text-align: justify; background-color: rgb(255, 255, 255); font-size: 16px; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">举例说明：</p>
		<pre class=""
			style="margin-top: 0px; margin-bottom: 0px; padding: 8px 0px 6px; max-width: 100%; box-sizing: border-box; letter-spacing: 0.544px; text-align: justify; background-color: rgb(47, 54, 64); border-radius: 0px; overflow-y: auto; color: rgb(80, 97, 109); font-size: 10px; line-height: 12px; word-wrap: break-word !important;">
			<ol class="list-paddingleft-2" style="list-style-type: none;">
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">SELECT * </span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> &nbsp;FROM user_info </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">as</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> i</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> &nbsp; &nbsp;LEFT JOIN user_account </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">as</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> a</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> &nbsp; &nbsp; &nbsp;ON i.userid = a.userid </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">and</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> i.userid = </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">;</span>
							</code></span>
					</p></li>
			</ol>
		</pre>
		<pre class=""
			style="margin-top: 0px; margin-bottom: 0px; padding: 8px 0px 6px; max-width: 100%; box-sizing: border-box; letter-spacing: 0.544px; text-align: justify; background-color: rgb(47, 54, 64); border-radius: 0px; overflow-y: auto; color: rgb(80, 97, 109); font-size: 10px; line-height: 12px; word-wrap: break-word !important;">
			<ol class="list-paddingleft-2" style="list-style-type: none;">
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">SELECT * </span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> &nbsp;FROM user_info </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">as</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> i</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> &nbsp; &nbsp;LEFT JOIN user_account </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">as</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> a</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> &nbsp; &nbsp; &nbsp;ON i.userid = a.userid </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">where</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> i.userid = </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">;</span>
							</code></span>
					</p></li>
			</ol>
		</pre>
		<p
			style="margin-top: 15px; margin-bottom: 15px; max-width: 100%; box-sizing: border-box; min-height: 1em; letter-spacing: 0.544px; text-align: justify; background-color: rgb(255, 255, 255); font-size: 16px; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">
			第一种情况<strong
				style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">LEFT
				JOIN</strong>在执行完第二步ON子句后，筛选出满足<strong
				style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">i.userid
				= a.userid and i.userid = 1003</strong>的行，生成表vt2，然后执行第三步JOIN子句，将外部行添加进虚拟表生成vt3即最终结果：
		</p>
		<pre class=""
			style="margin-top: 0px; margin-bottom: 0px; padding: 8px 0px 6px; max-width: 100%; box-sizing: border-box; letter-spacing: 0.544px; text-align: justify; background-color: rgb(47, 54, 64); border-radius: 0px; overflow-y: auto; color: rgb(80, 97, 109); font-size: 10px; line-height: 12px; word-wrap: break-word !important;">
			<ol class="list-paddingleft-2" style="list-style-type: none;">
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">vt2:</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| userid | name | userid | money |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | z &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">8</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">vt3:</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| userid | name | userid | money |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1001</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | x &nbsp; &nbsp;| &nbsp; NULL | &nbsp;NULL |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1002</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | y &nbsp; &nbsp;| &nbsp; NULL | &nbsp;NULL |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | z &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">8</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1004</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | a &nbsp; &nbsp;| &nbsp; NULL | &nbsp;NULL |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1005</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | b &nbsp; &nbsp;| &nbsp; NULL | &nbsp;NULL |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1006</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | c &nbsp; &nbsp;| &nbsp; NULL | &nbsp;NULL |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1007</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | d &nbsp; &nbsp;| &nbsp; NULL | &nbsp;NULL |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1008</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | e &nbsp; &nbsp;| &nbsp; NULL | &nbsp;NULL |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
			</ol>
		</pre>
		<p
			style="margin-top: 15px; margin-bottom: 15px; max-width: 100%; box-sizing: border-box; min-height: 1em; letter-spacing: 0.544px; text-align: justify; background-color: rgb(255, 255, 255); font-size: 16px; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">
			而第二种情况<strong
				style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">LEFT
				JOIN</strong>在执行完第二步ON子句后，筛选出满足<strong
				style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">i.userid
				= a.userid</strong>的行，生成表vt2；再执行第三步JOIN子句添加外部行生成表vt3；然后执行第四步WHERE子句，再对vt3表进行过滤生成vt4，得的最终结果：
		</p>
		<pre class=""
			style="margin-top: 0px; margin-bottom: 0px; padding: 8px 0px 6px; max-width: 100%; box-sizing: border-box; letter-spacing: 0.544px; text-align: justify; background-color: rgb(47, 54, 64); border-radius: 0px; overflow-y: auto; color: rgb(80, 97, 109); font-size: 10px; line-height: 12px; word-wrap: break-word !important;">
			<ol class="list-paddingleft-2" style="list-style-type: none;">
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">vt2:</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| userid | name | userid | money |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1001</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | x &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1001</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">22</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1002</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | y &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1002</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">30</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | z &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">8</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">vt3:</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| userid | name | userid | money |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1001</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | x &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1001</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">22</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1002</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | y &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1002</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp;</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">30</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | z &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">8</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1004</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | a &nbsp; &nbsp;| &nbsp; NULL | &nbsp;NULL |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1005</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | b &nbsp; &nbsp;| &nbsp; NULL | &nbsp;NULL |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1006</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | c &nbsp; &nbsp;| &nbsp; NULL | &nbsp;NULL |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1007</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | d &nbsp; &nbsp;| &nbsp; NULL | &nbsp;NULL |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1008</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | e &nbsp; &nbsp;| &nbsp; NULL | &nbsp;NULL |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">vt4:</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| userid | name | userid | money |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | z &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">8</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
			</ol>
		</pre>
		<p
			style="margin-top: 15px; margin-bottom: 15px; max-width: 100%; box-sizing: border-box; min-height: 1em; letter-spacing: 0.544px; text-align: justify; background-color: rgb(255, 255, 255); font-size: 16px; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">
			如果将上例的<strong
				style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">LEFT
				JOIN</strong>替换成<strong
				style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">INNER
				JOIN</strong>，不论将条件过滤放到<strong
				style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">ON</strong>还是<strong
				style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">WHERE</strong>里，结果都是一样的，因为<strong
				style="max-width: 100%; box-sizing: border-box; color: rgb(0, 0, 0); word-wrap: break-word !important;">INNER
				JOIN不会执行第三步添加外部行</strong>。
		</p>
		<pre class=""
			style="margin-top: 0px; margin-bottom: 0px; padding: 8px 0px 6px; max-width: 100%; box-sizing: border-box; letter-spacing: 0.544px; text-align: justify; background-color: rgb(47, 54, 64); border-radius: 0px; overflow-y: auto; color: rgb(80, 97, 109); font-size: 10px; line-height: 12px; word-wrap: break-word !important;">
			<ol class="list-paddingleft-2" style="list-style-type: none;">
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">SELECT * </span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> &nbsp;FROM user_info </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">as</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> i</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> &nbsp; &nbsp;INNER JOIN user_account </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">as</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> a</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> &nbsp; &nbsp; &nbsp;ON i.userid = a.userid </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">and</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> i.userid = </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">;</span>
							</code></span>
					</p></li>
			</ol>
		</pre>
		<pre class=""
			style="margin-top: 0px; margin-bottom: 0px; padding: 8px 0px 6px; max-width: 100%; box-sizing: border-box; letter-spacing: 0.544px; text-align: justify; background-color: rgb(47, 54, 64); border-radius: 0px; overflow-y: auto; color: rgb(80, 97, 109); font-size: 10px; line-height: 12px; word-wrap: break-word !important;">
			<ol class="list-paddingleft-2" style="list-style-type: none;">
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">SELECT * </span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> &nbsp;FROM user_info </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">as</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> i</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> &nbsp; &nbsp;INNER JOIN user_account </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">as</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> a</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> &nbsp; &nbsp; &nbsp;ON i.userid = a.userid </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(79, 193, 233); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">where</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> i.userid = </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">;</span>
							</code></span>
					</p></li>
			</ol>
		</pre>
		<p
			style="margin-top: 15px; margin-bottom: 15px; max-width: 100%; box-sizing: border-box; min-height: 1em; letter-spacing: 0.544px; text-align: justify; background-color: rgb(255, 255, 255); font-size: 16px; white-space: pre-line; line-height: 30px; color: rgb(74, 74, 74); font-family: Avenir, -apple-system-font, 微软雅黑, sans-serif; word-wrap: break-word !important;">返回结果都是：</p>
		<pre class=""
			style="margin-top: 0px; margin-bottom: 0px; padding: 8px 0px 6px; max-width: 100%; box-sizing: border-box; letter-spacing: 0.544px; text-align: justify; background-color: rgb(47, 54, 64); border-radius: 0px; overflow-y: auto; color: rgb(80, 97, 109); font-size: 10px; line-height: 12px; word-wrap: break-word !important;">
			<ol class="list-paddingleft-2" style="list-style-type: none;">
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| userid | name | userid | money |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | z &nbsp; &nbsp;| &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">1003</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> | &nbsp; &nbsp; </span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(172, 146, 236); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">8</span><span
									class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;"> |</span>
							</code></span>
					</p></li>
				<li><p
						style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
						<span
							style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); display: block; line-height: 22px; word-wrap: break-word !important; font-size: 14px !important; word-break: inherit !important;"><code
								style="margin-left: -20px; max-width: 100%; box-sizing: border-box; word-wrap: normal; display: flex; overflow: initial; line-height: 12px; border-width: 0px; border-style: initial; border-color: initial; font-size: 10px; font-family: inherit !important;">
								<span class=""
									style="max-width: 100%; box-sizing: border-box; color: rgb(230, 233, 237); line-height: 20px; word-wrap: break-word !important; font-size: 13px !important; white-space: inherit !important;">+--------+------+--------+-------+</span>
							</code></span>
					</p></li>
			</ol>
		</pre>
		<h4
			style="margin-top: 1.5rem; margin-bottom: 1rem; font-size: 18px; max-width: 100%; box-sizing: border-box;">
			<span
				style="max-width: 100%; color: rgb(204, 0, 0); box-sizing: border-box !important; word-wrap: break-word !important;"><strong
				style="max-width: 100%; box-sizing: border-box !important; word-wrap: break-word !important;">参考资料</strong></span>
		</h4>
		<ul class="list-paddingleft-2" style="list-style-type: square;">
			<li><p
					style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
					<span
						style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); line-height: 22px; word-wrap: break-word !important; font-size: 14px !important;">《MySQL技术内幕：SQL编程》</span>
				</p></li>
			<li><p
					style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
					<span
						style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); line-height: 22px; word-wrap: break-word !important; font-size: 14px !important;">SQL
						Joins - W3Schools</span>
				</p></li>
			<li><p
					style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
					<span
						style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); line-height: 22px; word-wrap: break-word !important; font-size: 14px !important;">sql
						- What is the difference between “INNER JOIN” and “OUTER JOIN”?</span>
				</p></li>
			<li><p
					style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
					<span
						style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); line-height: 22px; word-wrap: break-word !important; font-size: 14px !important;">MySQL
						:: MySQL 8.0 Reference Manual :: 13.2.10.2 JOIN Syntax</span>
				</p></li>
			<li><p
					style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
					<span
						style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); line-height: 22px; word-wrap: break-word !important; font-size: 14px !important;">Visual
						Representation of SQL Joins</span>
				</p></li>
			<li><p
					style="max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
					<span
						style="max-width: 100%; box-sizing: border-box; color: rgb(74, 74, 74); line-height: 22px; word-wrap: break-word !important; font-size: 14px !important;">Join
						(SQL) - Wikipedia</span>
				</p></li>
		</ul>
		<p
			style="white-space: normal; max-width: 100%; min-height: 1em; color: rgb(51, 51, 51);">
			<br>
		</p>
		<p
			style="white-space: normal; max-width: 100%; min-height: 1em; color: rgb(51, 51, 51);">
			<br>
		</p>
		<section class="" powered-by="xiumi.us"
			style="white-space: normal; max-width: 100%; box-sizing: border-box; color: rgb(51, 51, 51);">
			<section class=""
				style="margin-top: 10px; margin-bottom: 10px; max-width: 100%; box-sizing: border-box; word-wrap: break-word !important;">
				<section class=""
					style="padding: 10px; max-width: 100%; box-sizing: border-box; display: inline-block; width: 668px; border-width: 1px; border-style: solid; border-color: rgb(226, 226, 226); box-shadow: rgb(226, 226, 226) 0px 16px 1px -13px; word-wrap: break-word !important;">
					<section class="" powered-by="xiumi.us"
						style="max-width: 100%; box-sizing: border-box; word-wrap: break-word !important;">
						<section class=""
							style="max-width: 100%; box-sizing: border-box; word-wrap: break-word !important;">
							<section class=""
								style="max-width: 100%; box-sizing: border-box; word-wrap: break-word !important;">
								<p class=""
									style="max-width: 100%; box-sizing: border-box; min-height: 1em; color: rgb(93, 93, 93); font-size: 13px; word-wrap: break-word !important;">【关于投稿】</p>
								<p class=""
									style="max-width: 100%; box-sizing: border-box; min-height: 1em; color: rgb(93, 93, 93); font-size: 13px; word-wrap: break-word !important;">
									<br class=""
										style="max-width: 100%; box-sizing: border-box !important; word-wrap: break-word !important;">
								</p>
								<p class=""
									style="max-width: 100%; box-sizing: border-box; min-height: 1em; color: rgb(93, 93, 93); font-size: 13px; word-wrap: break-word !important;">如果大家有原创好文投稿，请直接给公号发送留言。</p>
								<p class=""
									style="max-width: 100%; box-sizing: border-box; min-height: 1em; color: rgb(93, 93, 93); font-size: 13px; word-wrap: break-word !important;">
									<br class=""
										style="max-width: 100%; box-sizing: border-box !important; word-wrap: break-word !important;">
								</p>
								<p class=""
									style="max-width: 100%; box-sizing: border-box; min-height: 1em; font-size: 13px; word-wrap: break-word !important;">
									<span class=""
										style="max-width: 100%; box-sizing: border-box !important; word-wrap: break-word !important;"><span
										class="" style="max-width: 100%; color: rgb(53, 53, 53);">①&nbsp;留言格式：</span><br
										class=""
										style="max-width: 100%; color: rgb(53, 53, 53); box-sizing: border-box !important; word-wrap: break-word !important;">
										<span class=""
										style="max-width: 100%; color: rgb(53, 53, 53);">【投稿】+《&nbsp;文章标题》+&nbsp;文章链接</span><br
										class=""
										style="max-width: 100%; color: rgb(53, 53, 53); box-sizing: border-box !important; word-wrap: break-word !important;">
										<br class=""
										style="max-width: 100%; color: rgb(53, 53, 53); box-sizing: border-box !important; word-wrap: break-word !important;">
										<span class=""
										style="max-width: 100%; color: rgb(53, 53, 53);">②&nbsp;示例：</span><br
										class=""
										style="max-width: 100%; color: rgb(53, 53, 53); box-sizing: border-box !important; word-wrap: break-word !important;">
										<span class=""
										style="max-width: 100%; color: rgb(53, 53, 53);">【投稿】</span></span><span
										class=""
										style="max-width: 100%; letter-spacing: 0.544px; box-sizing: border-box !important; word-wrap: break-word !important;">《不要自称是程序员，我十多年的
										IT 职场总结》：http://blog.jobbole.com/94148/</span>
								</p>
								<p class=""
									style="max-width: 100%; box-sizing: border-box; min-height: 1em; color: rgb(93, 93, 93); font-size: 13px; word-wrap: break-word !important;">
									<span class=""
										style="max-width: 100%; color: rgb(53, 53, 53); box-sizing: border-box !important; word-wrap: break-word !important;"><br
										class=""
										style="max-width: 100%; box-sizing: border-box !important; word-wrap: break-word !important;">③&nbsp;最后请附上您的个人简介哈~</span>
								</p>
								<p>
									<span class=""
										style="max-width: 100%; color: rgb(53, 53, 53); box-sizing: border-box !important; word-wrap: break-word !important;"><br></span>
								</p>
							</section>
						</section>
					</section>
				</section>
			</section>
		</section>
		<p
			style="white-space: normal; max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
			<span
				style="max-width: 100%; font-size: 14px; background-color: rgb(255, 254, 213); box-sizing: border-box !important; word-wrap: break-word !important;"></span><br>
		</p>
		<p
			style="white-space: normal; max-width: 100%; min-height: 1em; box-sizing: border-box !important; word-wrap: break-word !important;">
			<span
				style="max-width: 100%; font-size: 14px; background-color: rgb(255, 254, 213); box-sizing: border-box !important; word-wrap: break-word !important;"><br></span>
		</p>
		<p
			style="font-size: 16px; white-space: normal; max-width: 100%; min-height: 1em; color: rgb(62, 62, 62); background-color: rgb(255, 255, 255); text-align: center; box-sizing: border-box !important; word-wrap: break-word !important;">
			<span
				style="max-width: 100%; color: rgb(255, 169, 0); font-size: 15px; box-sizing: border-box !important; word-wrap: break-word !important;">看完本文有收获？请转发分享给更多人</span>
		</p>
		<p
			style="font-size: 16px; white-space: normal; max-width: 100%; min-height: 1em; color: rgb(62, 62, 62); background-color: rgb(255, 255, 255); line-height: 25.6px; text-align: center; box-sizing: border-box !important; word-wrap: break-word !important;">
			<span
				style="max-width: 100%; font-size: 15px; box-sizing: border-box !important; word-wrap: break-word !important;"><strong
				style="max-width: 100%; box-sizing: border-box !important; word-wrap: break-word !important;"><span
					style="max-width: 100%; color: rgb(255, 169, 0); box-sizing: border-box !important; word-wrap: break-word !important;">关注「数据分析与开发」，提升数据技能</span></strong></span>
		</p>
		<p
			style="font-size: 16px; white-space: normal; max-width: 100%; min-height: 1em; color: rgb(62, 62, 62); background-color: rgb(255, 255, 255); text-align: center; box-sizing: border-box !important; word-wrap: break-word !important;">
			<img class="" data-copyright="0" data-ratio="0.9166666666666666"
				data-s="300,640"
				data-src="https://mmbiz.qpic.cn/mmbiz_png/DmibiaFiaAI4B3YpcZYPicgc9JTMiaACNXE5A9FePsKgBic7LNlibx2fwVycTN4Wq47TzYXTNnP2PCKCVAGibNmzDnD0zg/640?wx_fmt=png"
				data-type="png" data-w="600" width="auto"
				style="box-sizing: border-box !important; word-wrap: break-word !important; visibility: visible !important; width: auto !important; height: auto !important;"
				_width="auto"
				src="https://mmbiz.qpic.cn/mmbiz_png/DmibiaFiaAI4B3YpcZYPicgc9JTMiaACNXE5A9FePsKgBic7LNlibx2fwVycTN4Wq47TzYXTNnP2PCKCVAGibNmzDnD0zg/640?wx_fmt=png&amp;tp=webp&amp;wxfrom=5&amp;wx_lazy=1&amp;wx_co=1"
				crossorigin="anonymous" data-fail="0">
		</p>
	</div>
	<script nonce="" type="text/javascript">
		var first_sceen__time = (+new Date()); 
		if ("" == 1 && document.getElementById('js_content')) {
			document.getElementById('js_content').addEventListener(
					"selectstart", function(e) {
						e.preventDefault();
					});
		} 
		(function() {
			if (navigator.userAgent.indexOf("WindowsWechat") != -1) {
				var link = document.createElement('link');
				var head = document.getElementsByTagName('head')[0];
				link.rel = 'stylesheet';
				link.type = 'text/css';
				link.href = "//res.wx.qq.com/mmbizwap/zh_CN/htmledition/style/page/appmsg_new/winwx3ec991.css";
				head.appendChild(link);
			}
		})();
	</script> 
	<div class="ct_mpda_wrp" id="js_sponsor_ad_area" style="display: none;"></div> 
	<div class="reward_area tc reward_area_primary"
		id="js_preview_reward_author" style="display: none;">
		<div class="reward-avatar" style="display: none;"
			id="js_preview_reward_author_avatar">
			<img src="" alt="" id="js_preview_reward_author_head">
		</div> 
		<div class="reward-author" id="js_preview_reward_author_name"></div>
		<p class="reward_tips" id="js_preview_reward_author_wording"
			style="display: none;"></p>
		<p>
			<a class="reward_button" id="js_preview_reward_author_link" href="##"><span
				id="js_preview_reward_link_text">赞赏</span></a>
		</p>
	</div> 
	<div class="reward_qrcode_area reward_area tc"
		id="js_preview_reward_qrcode" style="display: none;">
		<p class="tips_global">长按二维码向我转账</p>
		<p id="js_preview_reward_ios_wording" class="reward_tips"
			style="display: none;"></p>
		<span class="reward_qrcode_img_wrp"><img
			class="reward_qrcode_img"
			src="//res.wx.qq.com/mmbizwap/zh_CN/htmledition/images/pic/appmsg/pic_reward_qrcode.2x3534dd.png"></span>
		<p class="tips_global">受苹果公司新规定影响，微信 iOS 版的赞赏功能被关闭，可通过二维码转账支持公众号。</p>
	</div>


</div>
