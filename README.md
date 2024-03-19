# Project-Recell

**Business Context**

Buying and selling used phones and tablets used to be something that happened on a handful of online marketplace sites. But the used and refurbished device market has grown considerably over the past decade, and a new IDC (International Data Corporation) forecast predicts that the used phone market would be worth \$52.7bn by 2023 with a compound annual growth rate (CAGR) of 13.6% from 2018 to 2023. This growth can be attributed to an uptick in demand for used phones and tablets that offer considerable savings compared with new models.

Refurbished and used devices continue to provide cost-effective alternatives to both consumers and businesses that are looking to save money when purchasing one. There are plenty of other benefits associated with the used device market. Used and refurbished devices can be sold with warranties and can also be insured with proof of purchase. Third-party vendors/platforms, such as Verizon, Amazon, etc., provide attractive offers to customers for refurbished devices. Maximizing the longevity of devices through second-hand trade also reduces their environmental impact and helps in recycling and reducing waste. The impact of the COVID-19 outbreak may further boost this segment as consumers cut back on discretionary spending and buy phones and tablets only for immediate needs.

**Objective**

The rising potential of this comparatively under-the-radar market fuels the need for an ML-based solution to develop a dynamic pricing strategy for used and refurbished devices. ReCell, a startup aiming to tap the potential in this market, has hired you as a data scientist. They want you to analyze the data provided and build a linear regression model to predict the price of a used phone/tablet and identify factors that significantly influence it.

**Data Description**

The data contains the different attributes of used/refurbished phones and tablets. The data was collected in the year 2021. The detailed data dictionary is given below.

brand_name: Name of manufacturing brand

os: OS on which the device runs

screen_size: Size of the screen in cm

4g: Whether 4G is available or not

5g: Whether 5G is available or not

main_camera_mp: Resolution of the rear camera in megapixels

selfie_camera_mp: Resolution of the front camera in megapixels

int_memory: Amount of internal memory (ROM) in GB

ram: Amount of RAM in GB

battery: Energy capacity of the device battery in mAh

weight: Weight of the device in grams

release_year: Year when the device model was released

days_used: Number of days the used/refurbished device has been used

normalized_new_price: Normalized price of a new device of the same model in euros

normalized_used_price: Normalized price of the used/refurbished device in euros


**Actionable Insights**

The genearted linear regression model is able to explain ~84% of the variation in the used device data and within 4.5% of the normalized used price of the devices on the test data, which is really good. Hence the model is good for prediction as well as inference purposes.

The normalized used price increases by 0.0207 units for every unit increase of ram given all the other variables are held constant.

If the selfie camera megapixels increases by one unit, then the normalized used price of the devices increases by 0.0138 units given all the other variables are held constant.

If the weight of the used devices increases by one unit, then the normalized used price of the devices increases by 0.0017 units given all the other variables are held constant.

For every unit increase in year since the device was released, the normalized used price decreases by 0.0292 units given all the other variables are held constant.

If the normalized new price of the devices of the same model of the used device increases by one unit, then the noramlized used price of the devices increases by 0.4415 units given all the other variables are held constant.

The Karbonn brand devices increases the normalized used price by 0.1156 units given all the other variables are held constant.

The normalized used price for the devices of brands Samsung and Sony decreases by 0.0374 and 0.0670 units respectively considering all the other variables are constant.

The normalized used price of the devices running on OS other than windows, Andriod and ios gets decreased by 0.1276 units for every unit increase in the os considering that all the other variables are held constant.

If the used device is running on ios, then for every unit increase in the OS the normalized used price decreases by 0.09 units given all the other variables are held constant.

The normalized used price increases by 0.05 units if the used device has 4g data avaialbility.

**Business Recommendations**

The ReCell can consider procuring more used devices with large ram capacity in their online portal inorder to yield profit as the normalized used price of the devices increases with increase in the ram capacity.

Since the customers buying used devices has preferences on the resolution of the selfie camera and main camera, the ReCell can focus on selling used devices having more than 8mp selfie camera and more than 16mp main camera resolution to run the business in the successful path as well as to build customer satisfaction.

The ReCell business team has to consider the factor of 4g data availability while procuring and selling the used devices as the normalized used price increases when 4g data is available in the devices.

The ReCell needs to consider the age of the phone they are selling as the phones becomes older the normalized used price goes down. Hence the ReCell company can have more inventory of phones not more than 5 years old.
