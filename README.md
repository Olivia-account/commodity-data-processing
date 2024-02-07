# commodity-data-processing
这是关于招聘数据科学家的问题。需要创建一个模型来预测候选人在培训后是否会留在公司工作。这个任务需要使用候选人的个人信息和经历数据来预测他们留在公司工作的概率。同时，还需要解释模型如何影响候选人的决定。

数据的特征：
- enrollee_id: 候选人的唯一ID
- city: 城市代码
- city_development_index: 城市的发展指数（已缩放）
- gender: 候选人的性别
- relevent_experience: 候选人的相关经验
- enrolled_university: 如果有，候选人所注册的大学课程类型
- education_level: 候选人的教育水平
- major_discipline: 候选人的教育专业学科
- experience: 候选人的总工作经验年限
- company_size: 目前雇主公司的员工数量
- company_type: 目前雇主的公司类型
- last_new_job: 上一份工作和目前工作之间的年份差
- training_hours: 完成的培训小时数
- target: 0 – 不寻找工作变动，1 – 寻找工作变动

问题陈述：
- 预测候选人会为公司工作的概率
- 解释模型，阐明哪些特征影响了候选人的决定
