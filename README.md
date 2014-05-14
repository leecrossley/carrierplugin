<!---
    Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
    distributed with this work for additional information
    regarding copyright ownership.  The ASF licenses this file
    to you under the Apache License, Version 2.0 (the
    "License"); you may not use this file except in compliance
    with the License.  You may obtain a copy of the License at

      http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing,
    software distributed under the License is distributed on an
    "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
-->

# cn.edu.gdmec.t00385.cordova.carrier

这是个用于测试cordova Ver3.0的插件编写的案例，可以返回android手机的运营商名称。

## Installation 安装方法

    cordova plugin add https://github.com/gdmec/carrierplugin.git

## Supported Platforms

- Android

## Methods 调用方法

- navigator.Carrier.getCarrierCode(onSuccess, onFailure);



### Example

    <button onclick="test();">获取手机运营商</button>
    <script type="text/javascript">
        function test() {
            Carrier.getCarrierCode(onSuccess, onFailure);
        }
        function onSuccess(result) {
            alert("运营商: " + result);
        }
        function onFailure(err) {
            alert("Failure: " + err);
        }
    </script>
