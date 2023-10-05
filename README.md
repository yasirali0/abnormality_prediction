# Abnormality prediction for industrial air compressors

This repo is for [4th Special 2023 Research and Development Zone AI SPARK Challenge - Air compressor abnormality](https://aifactory.space/task/2226/overview).

In industrial air compressors and rotating machines, motor and core temperature, vibration, and noise are factors that affect device fatigue, and increased fatigue can cause equipment failure. <br/>

The goal is to develop a model that predicts signs of malfunction in industrial equipment through unsupervised learning, so that if fatigue increases, we would prevent equipment failure, and prevents accidents. <br/>

We used autoencoder model for this challenge, and secured 104th position on the leaderboard with a macro-F1 score of 0.9538864792.

### About Data
train_data : This is training data, which represents all normal cases. <br/>
test_data : This is data for evaluation and includes both normal and abnormal cases, and is subject to prediction. <br/>
answer_sample : Label file form for submission to be filled out for test_data. <br/>

1. Features <br/>
<b>air_inflow</b>: air intake flow rate (^3/min) <br/>
<b>air_end_temp</b>: Air end temperature (°C) <br/>
<b>out_pressure</b>: Discharge pressure (Mpa) <br/>
<b>motor_current</b>: motor current (A) <br/>
<b>motor_rpm</b>: Motor rotation speed (rpm) <br/>
<b>motor_temp</b>: motor temperature (°C) <br/>
<b>motor_vibe</b>: Motor vibration (mm/s) <br/>
<b>type</b>: Facility number <br/>

2. Additionally, each facility has the following characteristics. <br/>
<b>Facility number 0, 4, 5, 6, 7</b>: 30 HP (horsepower) <br/>
<b>Facility number 1</b>: 20HP <br/>
<b>Facility number 2</b>: 10HP <br/>
<b>Facility number 3</b>: 50HP <br/>
