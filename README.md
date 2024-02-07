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


以下是对每个特征进行编码的部分：

- 'gender'特征：将缺失值填充为0，然后使用字典映射将'Male'、'Female'和'Other'分别替换为1、2和3。
- 'relevent_experience'特征：使用字典映射将'Has relevent experience'和'No relevent experience'分别替换为1和2。
- 'enrolled_university'特征：将缺失值填充为0，然后使用字典映射将'no_enrollment'、'Full time course'和'Part time course'分别替换为1、2和3。
- 'education_level'特征：将缺失值填充为0，然后使用字典映射将'Graduate'、'Masters'、'High School'、'Phd'和'Primary School'分别替换为1、2、3、4和5。
- 'major_discipline'特征：将缺失值填充为0，然后使用字典映射将'STEM'、'Business Degree'、'Arts'、'Humanities'、'No Major'和'Other'分别替换为 1、2、3、4、5和6。
- 'experience'特征：将缺失值填充为0，然后使用字典映射将'>20'替换为25，'<1'替换为0.5，并将数据类型转换为浮点型。
- 'company_size'特征：使用字典映射将'<10'、'10/49'、'50-99'、'100-500'、'500-999'、'1000-4999'、'5000-9999'和'10000+'分别替换为5、30、75、- 300、750、3000、7500和15000，并将缺失值填充为0。
- 'company_type'特征：使用字典映射将'Pvt Ltd'、'Funded Startup'、'Public Sector'、'Early Stage Startup'、'NGO'和'Other'分别替换为1、2、3、4、5和6，并将缺失值填充为0。
- 'last_new_job'特征：使用字典映射将'>4'替换为5，'never'替换为0，并将缺失值填充为0，并将数据类型转换为浮点型。

![image](https://github.com/Olivia-account/commodity-data-processing/assets/60562899/51478457-ab3f-4ac1-bc98-a89fd9caf18c)

# 完整讲解
https://blog.csdn.net/m0_46573428/article/details/136068236
# 后记
如果觉得有帮助的话，求 关注、收藏、点赞、星星 哦！
