
# TikTokAPI接口，用户粉丝列表采集

> **针对开放隐私设置，关注/粉丝列表对外可见的用户有效**




**请求API：**
```http
http://主机地址/tk/user/followers?token=xxx&uid=6754915036232582149&cursor=1631063752
```


**请求方式：**
```http
GET
```

>**了解更多短视频直播数据采集分析接口请**[点击查看接口文档](https://docs.qq.com/doc/DU1VrcWR5ekZFYmJO) 

**参数：**

| 参数名 | 必选 | 类型 | 说明 |
| --- | --- | --- | --- |
| token | 是 | string | 接口授权码 |
| uid | 是 | int | 用户的user_id，非TK号，[点击查看获取方法](https://www.yuque.com/books/share/d37ad7e7-95b0-4535-ad74-2cb5f639e99f/opsoz9) |
| cursor | 否 | int | 翻页游标，根据结果返回的min_time传入作为下一页翻页参数，初始为0 |

​

**status_code状态码：**

| status_code**状态码** | **说明** |
| --- | --- |
| 2096 | 由于该用户隐私设置，列表不可见 |
| 2065 | 用户不存在 |

​

​

**返回示例**
```json
{
	"code": 200,
	"msg": "成功",
	"data": {
		"max_time": 1631063752,
		"min_time": 1631063752,
		"has_more": true,
		"myself_user_id": "0",
		"offset": 20,
		"extra": {
			"fatal_item_ids": [],
			"logid": "202109080115520102450220261546B838",
			"now": 1631063752000
		},
		"log_pb": {
			"impr_id": "202109080115520102450220261546B838"
		},
		"status_code": 0,
		"rec_has_more": true,
		"total": 8229668,
		"followers": [
			{
				"react_setting": 0,
				"stitch_setting": 0,
				"aweme_count": 0,
				"twitter_id": "",
				"user_canceled": false,
				"ins_id": "",
				"homepage_bottom_toast": null,
				"mutual_relation_avatars": null,
				"avatar_thumb": {
					"height": 720,
					"uri": "tiktok-obj\/7005362653325426689",
					"url_list": [
						"https:\/\/p16-sign-sg.tiktokcdn.com\/aweme\/100x100\/tiktok-obj\/7005362653325426689.webp?x-expires=1631149200&x-signature=VO80wq2dLYsKLeewVzFsiAU1wMI%3D",
						"https:\/\/p16-sign-sg.tiktokcdn.com\/aweme\/100x100\/tiktok-obj\/7005362653325426689.jpeg?x-expires=1631149200&x-signature=2sY5jKPzvlyQrtRBVgGvoiAeezw%3D"
					],
					"width": 720
				},
				"live_verify": 0,
				"enterprise_verify_reason": "",
				"follower_status": 0,
				"comment_setting": 0,
				"custom_verify": "",
				"avatar_medium": {
					"uri": "tiktok-obj\/7005362653325426689",
					"url_list": [
						"https:\/\/p16-sign-sg.tiktokcdn.com\/aweme\/720x720\/tiktok-obj\/7005362653325426689.webp?x-expires=1631149200&x-signature=ql2w6NkfY3jMIvWIHhQY5T5VFEY%3D",
						"https:\/\/p16-sign-sg.tiktokcdn.com\/aweme\/720x720\/tiktok-obj\/7005362653325426689.jpeg?x-expires=1631149200&x-signature=Qn18EA1MOLpPJM7YJM008XVGRRs%3D"
					],
					"width": 720,
					"height": 720
				},
				"bold_fields": null,
				"is_ad_fake": false,
				"has_email": false,
				"create_time": 0,
				"user_period": 0,
				"avatar_larger": {
					"uri": "tiktok-obj\/7005362653325426689",
					"url_list": [
						"https:\/\/p16-sign-sg.tiktokcdn.com\/aweme\/1080x1080\/tiktok-obj\/7005362653325426689.webp?x-expires=1631149200&x-signature=S2KtrGmhT68Tc88cKo0TKmrQEKM%3D",
						"https:\/\/p16-sign-sg.tiktokcdn.com\/aweme\/1080x1080\/tiktok-obj\/7005362653325426689.jpeg?x-expires=1631149200&x-signature=E8o3Ip3o1G9rsA8V53iRxBaQxfI%3D"
					],
					"width": 720,
					"height": 720
				},
				"has_facebook_token": false,
				"share_info": {
					"share_weibo_desc": "",
					"share_desc": "",
					"share_title": "",
					"share_qrcode_url": {
						"uri": "",
						"url_list": [],
						"width": 720,
						"height": 720
					},
					"share_title_myself": "",
					"share_title_other": "",
					"share_desc_info": "",
					"share_url": ""
				},
				"video_icon": {
					"url_list": [],
					"width": 720,
					"height": 720,
					"uri": ""
				},
				"cover_url": [
					{
						"uri": "tiktok-obj\/1613727517271041",
						"url_list": [
							"https:\/\/p16-sg.tiktokcdn.com\/obj\/tiktok-obj\/1613727517271041"
						],
						"width": 720,
						"height": 720
					}
				],
				"follow_status": 0,
				"room_id": 0,
				"total_favorited": 0,
				"with_fusion_shop_entry": false,
				"qa_status": 0,
				"youtube_channel_id": "",
				"live_agreement_time": 0,
				"avatar_uri": "tiktok-obj\/7005362653325426689",
				"short_id": "0",
				"user_rate": 1,
				"download_prompt_ts": 0,
				"language": "",
				"live_agreement": 0,
				"is_phone_binded": false,
				"reflow_page_uid": 0,
				"verify_info": "",
				"ad_cover_url": null,
				"tw_expire_time": 0,
				"shield_follow_notice": 0,
				"followers_detail": null,
				"gender": 0,
				"verification_type": 1,
				"events": null,
				"has_insights": false,
				"item_list": null,
				"youtube_channel_title": "",
				"status": 1,
				"live_commerce": false,
				"shield_digg_notice": 0,
				"platform_sync_info": null,
				"google_account": "",
				"reflow_page_gid": 0,
				"sec_uid": "MS4wLjABAAAAhjvKRC2R-0dLFbp-ycs9Pkr_ICiXbUVf2qTWQ9Qi4UsD-mJZl1Z1rWohOylie18T",
				"white_cover_url": null,
				"special_lock": 1,
				"commerce_user_level": 0,
				"prevent_download": false,
				"type_label": null,
				"search_highlight": null,
				"nickname": "mqyeq",
				"follower_count": 0,
				"bind_phone": "",
				"secret": 0,
				"user_tags": null,
				"with_commerce_entry": false,
				"with_shop_entry": false,
				"uid": "7005153156116071425",
				"show_image_bubble": false,
				"is_star": false,
				"avatar_300x300": {
					"height": 720,
					"uri": "tiktok-obj\/7005362653325426689",
					"url_list": [
						"https:\/\/p16-sign-sg.tiktokcdn.com\/tiktok-obj\/7005362653325426689~c5_300x300.webp?x-expires=1631149200&x-signature=KyRJqgqHimaqQ7Db0i2ZqO7sv3U%3D",
						"https:\/\/p16-sign-sg.tiktokcdn.com\/tiktok-obj\/7005362653325426689~c5_300x300.jpeg?x-expires=1631149200&x-signature=l9Ng%2BPpVJ5ap6Tv2mvYsCQ0m0n8%3D"
					],
					"width": 720
				},
				"favoriting_count": 0,
				"can_set_geofencing": null,
				"following_count": 3,
				"authority_status": 0,
				"twitter_name": "",
				"need_recommend": 0,
				"duet_setting": 0,
				"is_block": false,
				"hide_search": false,
				"comment_filter_status": 0,
				"original_musician": {
					"music_count": 0,
					"music_used_count": 0,
					"digg_count": 0
				},
				"accept_private_policy": false,
				"birthday": "1900-01-01",
				"has_twitter_token": false,
				"account_region": "",
				"download_setting": 0,
				"cha_list": null,
				"region": "CN",
				"user_mode": 1,
				"cv_level": "",
				"need_points": null,
				"shield_comment_notice": 0,
				"is_discipline_member": false,
				"unique_id_modify_time": 1631063752,
				"share_qrcode_uri": "",
				"signature": "",
				"unique_id": "mqyeq",
				"has_orders": false,
				"has_youtube_token": false,
				"youtube_expire_time": 0,
				"avatar_168x168": {
					"uri": "tiktok-obj\/7005362653325426689",
					"url_list": [
						"https:\/\/p16-sign-sg.tiktokcdn.com\/tiktok-obj\/7005362653325426689~c5_168x168.webp?x-expires=1631149200&x-signature=%2F4HhcPj1fwn%2FkFEOEWaKz%2F8p8HQ%3D",
						"https:\/\/p16-sign-sg.tiktokcdn.com\/tiktok-obj\/7005362653325426689~c5_168x168.jpeg?x-expires=1631149200&x-signature=NP8Dq4HhkhSpWwrqG2A7oMc2YNE%3D"
					],
					"width": 720,
					"height": 720
				},
				"apple_account": 0,
				"relative_users": null,
				"fb_expire_time": 0,
				"geofencing": []
			},
			{
				"avatar_medium": {
					"uri": "musically-maliva-obj\/6977509749222801414",
					"url_list": [
						"https:\/\/p16-sign-va.tiktokcdn.com\/musically-maliva-obj\/6977509749222801414~c5_720x720.webp?x-expires=1631149200&x-signature=ofVBSXfRNGAe71s0vIs5oIhH%2BYs%3D",
						"https:\/\/p16-sign-va.tiktokcdn.com\/musically-maliva-obj\/6977509749222801414~c5_720x720.jpeg?x-expires=1631149200&x-signature=WM5SwcfmsDDXZc4G4BLxkXE7Mxs%3D"
					],
					"width": 720,
					"height": 720
				},
				"live_commerce": false,
				"share_qrcode_uri": "",
				"relative_users": null,
				"youtube_channel_id": "",
				"youtube_channel_title": "",
				"favoriting_count": 4639,
				"has_youtube_token": false,
				"share_info": {
					"share_desc": "",
					"share_title": "",
					"share_qrcode_url": {
						"url_list": [],
						"width": 720,
						"height": 720,
						"uri": ""
					},
					"share_title_myself": "",
					"share_title_other": "",
					"share_desc_info": "",
					"share_url": "",
					"share_weibo_desc": ""
				},
				"video_icon": {
					"uri": "",
					"url_list": [],
					"width": 720,
					"height": 720
				},
				"room_id": 0,
				"comment_setting": 0,
				"hide_search": false,
				"has_facebook_token": false,
				"tw_expire_time": 0,
				"user_mode": 1,
				"with_shop_entry": false,
				"white_cover_url": null,
				"nickname": "liajoseph5",
				"signature": "",
				"custom_verify": "",
				"commerce_user_level": 0,
				"cover_url": [
					{
						"uri": "tiktok-obj\/1613727517271041",
						"url_list": [
							"https:\/\/p16-sg.tiktokcdn.com\/obj\/tiktok-obj\/1613727517271041"
						],
						"width": 720,
						"height": 720
					}
				],
				"type_label": null,
				"uid": "6977504145574577157",
				"gender": 0,
				"avatar_uri": "musically-maliva-obj\/6977509749222801414",
				"cv_level": "",
				"download_setting": 0,
				"download_prompt_ts": 0,
				"has_insights": false,
				"aweme_count": 0,
				"unique_id": "liajoseph5",
				"has_email": false,
				"create_time": 0,
				"shield_digg_notice": 0,
				"has_twitter_token": false,
				"accept_private_policy": false,
				"status": 1,
				"show_image_bubble": false,
				"follower_status": 0,
				"sec_uid": "MS4wLjABAAAAkZDGdPES3JzrODS204l5uiMKxch6KsoigWIOPjSPj01sZRXts4mejbwK3d-MS9mg",
				"following_count": 255,
				"live_verify": 0,
				"verification_type": 1,
				"is_ad_fake": false,
				"followers_detail": null,
				"bind_phone": "",
				"shield_comment_notice": 0,
				"twitter_id": "",
				"need_recommend": 0,
				"youtube_expire_time": 0,
				"unique_id_modify_time": 1631063752,
				"google_account": "",
				"authority_status": 0,
				"ins_id": "",
				"avatar_300x300": {
					"uri": "musically-maliva-obj\/6977509749222801414",
					"url_list": [
						"https:\/\/p16-sign-va.tiktokcdn.com\/musically-maliva-obj\/6977509749222801414~c5_300x300.webp?x-expires=1631149200&x-signature=8F2d7%2FndzKk5Q1e%2FhpnuWYw3iIQ%3D",
						"https:\/\/p16-sign-va.tiktokcdn.com\/musically-maliva-obj\/6977509749222801414~c5_300x300.jpeg?x-expires=1631149200&x-signature=xjhIp7WCmVZ4zTNABCQsjV9RopU%3D"
					],
					"width": 720,
					"height": 720
				},
				"qa_status": 0,
				"can_set_geofencing": null,
				"bold_fields": null,
				"prevent_download": false,
				"user_canceled": false,
				"duet_setting": 0,
				"avatar_168x168": {
					"uri": "musically-maliva-obj\/6977509749222801414",
					"url_list": [
						"https:\/\/p16-sign-va.tiktokcdn.com\/musically-maliva-obj\/6977509749222801414~c5_168x168.webp?x-expires=1631149200&x-signature=e1e12RHGEKKn3ZaT%2FzKyoIOzjYo%3D",
						"https:\/\/p16-sign-va.tiktokcdn.com\/musically-maliva-obj\/6977509749222801414~c5_168x168.jpeg?x-expires=1631149200&x-signature=K0Y7aNjrQh6TOkpWD9SX3GUbw4w%3D"
					],
					"width": 720,
					"height": 720
				},
				"original_musician": {
					"music_count": 0,
					"music_used_count": 0,
					"digg_count": 0
				},
				"enterprise_verify_reason": "",
				"is_discipline_member": false,
				"fb_expire_time": 0,
				"apple_account": 0,
				"comment_filter_status": 0,
				"reflow_page_gid": 0,
				"ad_cover_url": null,
				"region": "CN",
				"geofencing": [],
				"is_block": false,
				"user_rate": 1,
				"need_points": null,
				"is_star": false,
				"homepage_bottom_toast": null,
				"live_agreement": 0,
				"user_period": 0,
				"reflow_page_uid": 0,
				"react_setting": 0,
				"stitch_setting": 0,
				"item_list": null,
				"live_agreement_time": 0,
				"follower_count": 21,
				"special_lock": 1,
				"account_region": "",
				"avatar_larger": {
					"uri": "musically-maliva-obj\/6977509749222801414",
					"url_list": [
						"https:\/\/p16-sign-va.tiktokcdn.com\/musically-maliva-obj\/6977509749222801414~c5_1080x1080.webp?x-expires=1631149200&x-signature=ule8usJZuoWG45kf2SO9NUYG3Ds%3D",
						"https:\/\/p16-sign-va.tiktokcdn.com\/musically-maliva-obj\/6977509749222801414~c5_1080x1080.jpeg?x-expires=1631149200&x-signature=GJHMzp7XOFJa5axyJza2aXr2u5g%3D"
					],
					"width": 720,
					"height": 720
				},
				"avatar_thumb": {
					"uri": "musically-maliva-obj\/6977509749222801414",
					"url_list": [
						"https:\/\/p16-sign-va.tiktokcdn.com\/musically-maliva-obj\/6977509749222801414~c5_100x100.webp?x-expires=1631149200&x-signature=C%2BahaKoeqRXfWGZq49E9r%2FLUmXc%3D",
						"https:\/\/p16-sign-va.tiktokcdn.com\/musically-maliva-obj\/6977509749222801414~c5_100x100.jpeg?x-expires=1631149200&x-signature=xiL3sxAbffZadHzzJdvkZPYI4HE%3D"
					],
					"width": 720,
					"height": 720
				},
				"shield_follow_notice": 0,
				"events": null,
				"cha_list": null,
				"birthday": "1900-01-01",
				"verify_info": "",
				"with_commerce_entry": false,
				"short_id": "0",
				"with_fusion_shop_entry": false,
				"twitter_name": "",
				"user_tags": null,
				"platform_sync_info": null,
				"has_orders": false,
				"is_phone_binded": false,
				"language": "",
				"secret": 0,
				"search_highlight": null,
				"follow_status": 0,
				"total_favorited": 0,
				"mutual_relation_avatars": null
			},
			{
				"need_recommend": 0,
				"share_info": {
					"share_desc_info": "",
					"share_url": "",
					"share_weibo_desc": "",
					"share_desc": "",
					"share_title": "",
					"share_qrcode_url": {
						"width": 720,
						"height": 720,
						"uri": "",
						"url_list": []
					},
					"share_title_myself": "",
					"share_title_other": ""
				},
				"account_region": "",
				"is_discipline_member": false,
				"is_phone_binded": false,
				"user_mode": 1,
				"cha_list": null,
				"aweme_count": 0,
				"live_agreement_time": 0,
				"ad_cover_url": null,
				"mutual_relation_avatars": null,
				"has_youtube_token": false,
				"twitter_id": "",
				"follower_status": 0,
				"relative_users": null,
				"user_tags": null,
				"youtube_channel_title": "",
				"apple_account": 0,
				"share_qrcode_uri": "",
				"homepage_bottom_toast": null,
				"with_commerce_entry": false,
				"live_agreement": 0,
				"platform_sync_info": null,
				"with_shop_entry": false,
				"reflow_page_uid": 0,
				"events": null,
				"signature": "",
				"user_rate": 1,
				"avatar_300x300": {
					"height": 720,
					"uri": "musically-maliva-obj\/6955545487436939270",
					"url_list": [
						"https:\/\/p16-sign-va.tiktokcdn.com\/musically-maliva-obj\/6955545487436939270~c5_300x300.webp?x-expires=1631149200&x-signature=Lj2Ncl%2FS47Syvth7m8xRp312NsA%3D",
						"https:\/\/p16-sign-va.tiktokcdn.com\/musically-maliva-obj\/6955545487436939270~c5_300x300.jpeg?x-expires=1631149200&x-signature=EY3yP%2Bor0q18Z4CdS8GhoALihTc%3D"
					],
					"width": 720
				},
				"total_favorited": 0,
				"is_block": false,
				"authority_status": 0,
				"user_canceled": false,
				"avatar_larger": {
					"uri": "musically-maliva-obj\/6955545487436939270",
					"url_list": [
						"https:\/\/p16-sign-va.tiktokcdn.com\/musically-maliva-obj\/6955545487436939270~c5_1080x1080.webp?x-expires=1631149200&x-signature=KM8WhQq3np%2FkpgcI353%2B%2FduiZVM%3D",
						"https:\/\/p16-sign-va.tiktokcdn.com\/musically-maliva-obj\/6955545487436939270~c5_1080x1080.jpeg?x-expires=1631149200&x-signature=PktmDzeRbWjaVt5Qo%2BHo2flfFs8%3D"
					],
					"width": 720,
					"height": 720
				},
				"followers_detail": null,
				"user_period": 0,
				"bold_fields": null,
				"has_twitter_token": false,
				"room_id": 0,
				"sec_uid": "MS4wLjABAAAAGhpNDj3iLfwfJlkwdA1tgm5dK1k_j-4JiJ2CTnw_4heBalAWnQl_jOK28un6BNpa",
				"gender": 0,
				"follow_status": 0,
				"shield_digg_notice": 0,
				"enterprise_verify_reason": "",
				"avatar_medium": {
					"uri": "musically-maliva-obj\/6955545487436939270",
					"url_list": [
						"https:\/\/p16-sign-va.tiktokcdn.com\/musically-maliva-obj\/6955545487436939270~c5_720x720.webp?x-expires=1631149200&x-signature=DGQ6ZjMNJqAHKZw%2FkaEY30L7J3Y%3D",
						"https:\/\/p16-sign-va.tiktokcdn.com\/musically-maliva-obj\/6955545487436939270~c5_720x720.jpeg?x-expires=1631149200&x-signature=96iLiqfYIlZd45jk8rdZ%2Bd%2BtGVs%3D"
					],
					"width": 720,
					"height": 720
				},
				"short_id": "0",
				"has_insights": false,
				"verification_type": 1,
				"shield_follow_notice": 0,
				"unique_id_modify_time": 1631063752,
				"with_fusion_shop_entry": false,
				"reflow_page_gid": 0,
				"type_label": null,
				"qa_status": 0,
				"custom_verify": "",
				"cover_url": [
					{
						"uri": "tiktok-obj\/1613727517271041",
						"url_list": [
							"https:\/\/p16-sg.tiktokcdn.com\/obj\/tiktok-obj\/1613727517271041"
						],
						"width": 720,
						"height": 720
					}
				],
				"stitch_setting": 0,
				"shield_comment_notice": 0,
				"tw_expire_time": 0,
				"ins_id": "",
				"cv_level": "",
				"search_highlight": null,
				"special_lock": 1,
				"show_image_bubble": false,
				"duet_setting": 0,
				"has_facebook_token": false,
				"has_orders": false,
				"geofencing": [],
				"video_icon": {
					"uri": "",
					"url_list": [],
					"width": 720,
					"height": 720
				},
				"google_account": "",
				"status": 1,
				"avatar_thumb": {
					"url_list": [
						"https:\/\/p16-sign-va.tiktokcdn.com\/musically-maliva-obj\/6955545487436939270~c5_100x100.webp?x-expires=1631149200&x-signature=pOjC%2B14HWOH4MA8liPruvB%2FgcWM%3D",
						"https:\/\/p16-sign-va.tiktokcdn.com\/musically-maliva-obj\/6955545487436939270~c5_100x100.jpeg?x-expires=1631149200&x-signature=XqZjxXsM%2B1ya1MOWasIUeQy1IE8%3D"
					],
					"width": 720,
					"height": 720,
					"uri": "musically-maliva-obj\/6955545487436939270"
				},
				"is_star": false,
				"nickname": "petaweta7",
				"original_musician": {
					"music_count": 0,
					"music_used_count": 0,
					"digg_count": 0
				},
				"live_commerce": false,
				"item_list": null,
				"bind_phone": "",
				"can_set_geofencing": null,
				"avatar_168x168": {
					"url_list": [
						"https:\/\/p16-sign-va.tiktokcdn.com\/musically-maliva-obj\/6955545487436939270~c5_168x168.webp?x-expires=1631149200&x-signature=tN9h%2BzCb4JZLKScp2B4ekMxo7Wc%3D",
						"https:\/\/p16-sign-va.tiktokcdn.com\/musically-maliva-obj\/6955545487436939270~c5_168x168.jpeg?x-expires=1631149200&x-signature=i4AL4sJkz5JMa7e%2B%2BXAal2%2FgQNw%3D"
					],
					"width": 720,
					"height": 720,
					"uri": "musically-maliva-obj\/6955545487436939270"
				},
				"is_ad_fake": false,
				"commerce_user_level": 0,
				"has_email": false,
				"create_time": 0,
				"birthday": "1900-01-01",
				"need_points": null,
				"youtube_expire_time": 0,
				"comment_setting": 0,
				"download_setting": 0,
				"download_prompt_ts": 0,
				"verify_info": "",
				"secret": 0,
				"youtube_channel_id": "",
				"accept_private_policy": false,
				"fb_expire_time": 0,
				"region": "US",
				"react_setting": 0,
				"uid": "6955544834803680262",
				"follower_count": 52,
				"hide_search": false,
				"unique_id": "petaweta7",
				"live_verify": 0,
				"comment_filter_status": 0,
				"following_count": 1705,
				"prevent_download": false,
				"twitter_name": "",
				"avatar_uri": "musically-maliva-obj\/6955545487436939270",
				"white_cover_url": null,
				"favoriting_count": 4342,
				"language": "en"
			},
			{
				"short_id": "0",
				"birthday": "1900-01-01",
				"total_favorited": 0,
				"live_agreement_time": 0,
				"create_time": 0,
				"type_label": null,
				"avatar_168x168": {
					"height": 720,
					"uri": "tos-maliva-avt-0068\/491dce28f18e5fef7aa6eb41290170a4",
					"url_list": [
						"https:\/\/p16-sign-va.tiktokcdn.com\/tos-maliva-avt-0068\/491dce28f18e5fef7aa6eb41290170a4~c5_168x168.webp?x-expires=1631149200&x-signature=uvWBpex7ggzYA%2BHR5%2FMXN0PnNGo%3D",
						"https:\/\/p16-sign-va.tiktokcdn.com\/tos-maliva-avt-0068\/491dce28f18e5fef7aa6eb41290170a4~c5_168x168.jpeg?x-expires=1631149200&x-signature=OUX0mrYRww85VZE1tJbWt6mv2mY%3D"
					],
					"width": 720
				},
				"enterprise_verify_reason": "",
				"platform_sync_info": null,
				"apple_account": 0,
				"avatar_uri": "tos-maliva-avt-0068\/491dce28f18e5fef7aa6eb41290170a4",
				"following_count": 18,
				"share_info": {
					"share_title_other": "",
					"share_desc_info": "",
					"share_url": "",
					"share_weibo_desc": "",
					"share_desc": "",
					"share_title": "",
					"share_qrcode_url": {
						"uri": "",
						"url_list": [],
						"width": 720,
						"height": 720
					},
					"share_title_myself": ""
				},
				"prevent_download": false,
				"stitch_setting": 0,
				"fb_expire_time": 0,
				"youtube_expire_time": 0,
				"is_ad_fake": false,
				"account_region": "",
				"google_account": "",
				"download_setting": 0,
				"search_highlight": null,
				"twitter_name": "",
				"react_setting": 0,
				"qa_status": 0,
				"uid": "6873525031273481222",
				"shield_follow_notice": 0,
				"live_agreement": 0,
				"with_shop_entry": false,
				"avatar_300x300": {
					"url_list": [
						"https:\/\/p16-sign-va.tiktokcdn.com\/tos-maliva-avt-0068\/491dce28f18e5fef7aa6eb41290170a4~c5_300x300.webp?x-expires=1631149200&x-signature=M2aRIXXd4Yc2dw8mxdU1suZ4JNk%3D",
						"https:\/\/p16-sign-va.tiktokcdn.com\/tos-maliva-avt-0068\/491dce28f18e5fef7aa6eb41290170a4~c5_300x300.jpeg?x-expires=1631149200&x-signature=GdvBHSeHyXHcKNtZPUfGU4ycXlw%3D"
					],
					"width": 720,
					"height": 720,
					"uri": "tos-maliva-avt-0068\/491dce28f18e5fef7aa6eb41290170a4"
				},
				"follower_count": 1,
				"item_list": null,
				"white_cover_url": null,
				"is_block": false,
				"shield_comment_notice": 0,
				"with_commerce_entry": false,
				"video_icon": {
					"uri": "",
					"url_list": [],
					"width": 720,
					"height": 720
				},
				"has_email": false,
				"reflow_page_gid": 0,
				"download_prompt_ts": 0,
				"avatar_medium": {
					"width": 720,
					"height": 720,
					"uri": "tos-maliva-avt-0068\/491dce28f18e5fef7aa6eb41290170a4",
					"url_list": [
						"https:\/\/p16-sign-va.tiktokcdn.com\/tos-maliva-avt-0068\/491dce28f18e5fef7aa6eb41290170a4~c5_720x720.webp?x-expires=1631149200&x-signature=UfD09BUWqgqafkeS10Id2oSPyyc%3D",
						"https:\/\/p16-sign-va.tiktokcdn.com\/tos-maliva-avt-0068\/491dce28f18e5fef7aa6eb41290170a4~c5_720x720.jpeg?x-expires=1631149200&x-signature=zXrUK6VsP19oNmFtxjo1LHxymNQ%3D"
					]
				},
				"user_rate": 1,
				"cover_url": [
					{
						"uri": "tiktok-obj\/1613727517271041",
						"url_list": [
							"https:\/\/p16-sg.tiktokcdn.com\/obj\/tiktok-obj\/1613727517271041"
						],
						"width": 720,
						"height": 720
					}
				],
				"relative_users": null,
				"unique_id_modify_time": 1631063752,
				"with_fusion_shop_entry": false,
				"user_mode": 1,
				"verification_type": 1,
				"commerce_user_level": 0,
				"nickname": "bored_at._h.ome",
				"need_recommend": 0,
				"original_musician": {
					"music_count": 0,
					"music_used_count": 0,
					"digg_count": 0
				},
				"special_lock": 1,
				"show_image_bubble": false,
				"is_phone_binded": false,
				"share_qrcode_uri": "",
				"room_id": 0,
				"status": 1,
				"cv_level": "",
				"tw_expire_time": 0,
				"followers_detail": null,
				"custom_verify": "",
				"bind_phone": "",
				"authority_status": 0,
				"ad_cover_url": null,
				"has_orders": false,
				"language": "en",
				"is_star": false,
				"bold_fields": null,
				"live_verify": 0,
				"can_set_geofencing": null,
				"sec_uid": "MS4wLjABAAAA_tmrF_COXlFvfvN8JH-JLlSwS8t1NVGfgI4Wgha3eYL39YyRwVixXcakWPnJeswI",
				"gender": 0,
				"is_discipline_member": false,
				"secret": 0,
				"live_commerce": false,
				"follow_status": 0,
				"favoriting_count": 32,
				"unique_id": "bored_at._h.ome",
				"has_youtube_token": false,
				"geofencing": [],
				"accept_private_policy": false,
				"user_canceled": false,
				"duet_setting": 0,
				"has_insights": false,
				"user_period": 0,
				"signature": "",
				"aweme_count": 0,
				"hide_search": false,
				"verify_info": "",
				"comment_setting": 0,
				"avatar_thumb": {
					"uri": "tos-maliva-avt-0068\/491dce28f18e5fef7aa6eb41290170a4",
					"url_list": [
						"https:\/\/p16-sign-va.tiktokcdn.com\/tos-maliva-avt-0068\/491dce28f18e5fef7aa6eb41290170a4~c5_100x100.webp?x-expires=1631149200&x-signature=OBA%2Bnb6QdVDaR8OvrWv%2FZxchTHI%3D",
						"https:\/\/p16-sign-va.tiktokcdn.com\/tos-maliva-avt-0068\/491dce28f18e5fef7aa6eb41290170a4~c5_100x100.jpeg?x-expires=1631149200&x-signature=kjsl4N34uMFihlUv3Sv3ieLiMO8%3D"
					],
					"width": 720,
					"height": 720
				},
				"follower_status": 0,
				"reflow_page_uid": 0,
				"need_points": null,
				"avatar_larger": {
					"uri": "tos-maliva-avt-0068\/491dce28f18e5fef7aa6eb41290170a4",
					"url_list": [
						"https:\/\/p16-sign-va.tiktokcdn.com\/tos-maliva-avt-0068\/491dce28f18e5fef7aa6eb41290170a4~c5_1080x1080.webp?x-expires=1631149200&x-signature=sTF6I2NYRVUxd7opniBScUeTuGI%3D",
						"https:\/\/p16-sign-va.tiktokcdn.com\/tos-maliva-avt-0068\/491dce28f18e5fef7aa6eb41290170a4~c5_1080x1080.jpeg?x-expires=1631149200&x-signature=eyMEjeBSJDQUGw8%2Bn8f7EPOmq1Y%3D"
					],
					"width": 720,
					"height": 720
				},
				"has_twitter_token": false,
				"cha_list": null,
				"homepage_bottom_toast": null,
				"youtube_channel_title": "",
				"region": "US",
				"mutual_relation_avatars": null,
				"twitter_id": "",
				"events": null,
				"ins_id": "",
				"comment_filter_status": 0,
				"user_tags": null,
				"has_facebook_token": false,
				"shield_digg_notice": 0,
				"youtube_channel_id": ""
			},
			{
				"region": "NZ",
				"prevent_download": false,
				"has_insights": false,
				"avatar_300x300": {
					"uri": "tos-alisg-avt-0068\/33e0b426411baaccf6d1144a8c684bb9",
					"url_list": [
						"https:\/\/p16-sign-sg.tiktokcdn.com\/tos-alisg-avt-0068\/33e0b426411baaccf6d1144a8c684bb9~c5_300x300.webp?x-expires=1631149200&x-signature=h1caeXN9pHrFxvAkGbQQJoJBBa4%3D",
						"https:\/\/p16-sign-sg.tiktokcdn.com\/tos-alisg-avt-0068\/33e0b426411baaccf6d1144a8c684bb9~c5_300x300.jpeg?x-expires=1631149200&x-signature=OzpBrX7L301Hc3sHcq%2BdaPJxp4E%3D"
					],
					"width": 720,
					"height": 720
				},
				"follower_count": 25,
				"hide_search": false,
				"room_data": "",
				"create_time": 0,
				"sec_uid": "MS4wLjABAAAAxd0RvxnvVcy-H7DT9ziEI1QbExjg_fhsc8FJVM2PTAp8GAcx-TsiidwEN651Hsfq",
				"has_email": false,
				"comment_setting": 0,
				"user_rate": 1,
				"nickname": "Trippy💨",
				"custom_verify": "",
				"secret": 1,
				"geofencing": [],
				"special_lock": 1,
				"account_region": "",
				"live_agreement_time": 0,
				"avatar_uri": "tos-alisg-avt-0068\/33e0b426411baaccf6d1144a8c684bb9",
				"reflow_page_uid": 0,
				"item_list": null,
				"white_cover_url": null,
				"avatar_larger": {
					"uri": "tos-alisg-avt-0068\/33e0b426411baaccf6d1144a8c684bb9",
					"url_list": [
						"https:\/\/p16-sign-sg.tiktokcdn.com\/aweme\/1080x1080\/tos-alisg-avt-0068\/33e0b426411baaccf6d1144a8c684bb9.webp?x-expires=1631149200&x-signature=S%2Bkj9Qfu%2BDxdN%2BOnypOJoYdKWqk%3D",
						"https:\/\/p16-sign-sg.tiktokcdn.com\/aweme\/1080x1080\/tos-alisg-avt-0068\/33e0b426411baaccf6d1144a8c684bb9.jpeg?x-expires=1631149200&x-signature=f111OrbeCfiwaKcy%2BrcZHywrH74%3D"
					],
					"width": 720,
					"height": 720
				},
				"shield_follow_notice": 0,
				"type_label": null,
				"followers_detail": null,
				"commerce_user_level": 0,
				"shield_comment_notice": 0,
				"with_commerce_entry": false,
				"is_ad_fake": false,
				"platform_sync_info": null,
				"show_image_bubble": false,
				"with_fusion_shop_entry": false,
				"short_id": "0",
				"aweme_count": 0,
				"relative_users": null,
				"bold_fields": null,
				"mutual_relation_avatars": null,
				"share_qrcode_uri": "",
				"user_mode": 1,
				"live_agreement": 0,
				"with_shop_entry": false,
				"unique_id_modify_time": 1630408930,
				"is_phone_binded": false,
				"follower_status": 0,
				"user_tags": null,
				"following_count": 237,
				"enterprise_verify_reason": "",
				"authority_status": 0,
				"status": 1,
				"download_setting": 3,
				"live_commerce": false,
				"follow_status": 0,
				"favoriting_count": 0,
				"original_musician": {
					"music_count": 0,
					"music_used_count": 0,
					"digg_count": 0
				},
				"video_icon": {
					"height": 720,
					"uri": "",
					"url_list": [],
					"width": 720
				},
				"cv_level": "",
				"ad_cover_url": null,
				"signature": "",
				"birthday": "1900-01-01",
				"share_info": {
					"share_url": "",
					"share_weibo_desc": "",
					"share_desc": "",
					"share_title": "",
					"share_qrcode_url": {
						"uri": "",
						"url_list": [],
						"width": 720,
						"height": 720
					},
					"share_title_myself": "",
					"share_title_other": "",
					"share_desc_info": ""
				},
				"stitch_setting": 3,
				"avatar_medium": {
					"uri": "tos-alisg-avt-0068\/33e0b426411baaccf6d1144a8c684bb9",
					"url_list": [
						"https:\/\/p16-sign-sg.tiktokcdn.com\/aweme\/720x720\/tos-alisg-avt-0068\/33e0b426411baaccf6d1144a8c684bb9.webp?x-expires=1631149200&x-signature=UoVxQgWlZyEyLPirXcvWImO3Oi4%3D",
						"https:\/\/p16-sign-sg.tiktokcdn.com\/aweme\/720x720\/tos-alisg-avt-0068\/33e0b426411baaccf6d1144a8c684bb9.jpeg?x-expires=1631149200&x-signature=n1X%2BkxxWt0NMnjpejAn84YBDdEU%3D"
					],
					"width": 720,
					"height": 720
				},
				"verify_info": "",
				"is_discipline_member": false,
				"is_star": false,
				"cha_list": null,
				"can_set_geofencing": null,
				"search_highlight": null,
				"need_recommend": 0,
				"live_verify": 0,
				"bind_phone": "",
				"cover_url": [
					{
						"url_list": [
							"https:\/\/p16-sg.tiktokcdn.com\/obj\/tiktok-obj\/1613727517271041"
						],
						"width": 720,
						"height": 720,
						"uri": "tiktok-obj\/1613727517271041"
					}
				],
				"language": "en",
				"comment_filter_status": 0,
				"need_points": null,
				"homepage_bottom_toast": null,
				"total_favorited": 0,
				"unique_id": "t.aylor298",
				"events": null,
				"react_setting": 3,
				"avatar_168x168": {
					"uri": "tos-alisg-avt-0068\/33e0b426411baaccf6d1144a8c684bb9",
					"url_list": [
						"https:\/\/p16-sign-sg.tiktokcdn.com\/tos-alisg-avt-0068\/33e0b426411baaccf6d1144a8c684bb9~c5_168x168.webp?x-expires=1631149200&x-signature=Eu%2FysP55vNFkZ0Y%2FGRGX93xpJqk%3D",
						"https:\/\/p16-sign-sg.tiktokcdn.com\/tos-alisg-avt-0068\/33e0b426411baaccf6d1144a8c684bb9~c5_168x168.jpeg?x-expires=1631149200&x-signature=LH6AdjggMYGpz%2FaN0%2FsqsBkj8hA%3D"
					],
					"width": 720,
					"height": 720
				},
				"avatar_thumb": {
					"height": 720,
					"uri": "tos-alisg-avt-0068\/33e0b426411baaccf6d1144a8c684bb9",
					"url_list": [
						"https:\/\/p16-sign-sg.tiktokcdn.com\/aweme\/100x100\/tos-alisg-avt-0068\/33e0b426411baaccf6d1144a8c684bb9.webp?x-expires=1631149200&x-signature=6VTCNNkhRg8jmltSqGELkaTfZ7o%3D",
						"https:\/\/p16-sign-sg.tiktokcdn.com\/aweme\/100x100\/tos-alisg-avt-0068\/33e0b426411baaccf6d1144a8c684bb9.jpeg?x-expires=1631149200&x-signature=d%2FRMDPzJVmOPKk%2BFBhtVsYCWy2k%3D"
					],
					"width": 720
				},
				"duet_setting": 3,
				"shield_digg_notice": 0,
				"has_orders": false,
				"user_canceled": false,
				"user_period": 0,
				"uid": "6970476749725434881",
				"is_block": false,
				"accept_private_policy": false,
				"reflow_page_gid": 0,
				"download_prompt_ts": 1622942284,
				"gender": 0,
				"verification_type": 1
			}
		]
	}
}
```
