# 使用限制

#### 专线连接的相关限制

- 专线连接对客户侧设备的要求，详见产品概述。
- 专线连接服务仅支持连接到同地域的边界网关，即物理连接和边界网关属于同一地域。
- 使用专线连接前，应规划好IDC内和VPC内的网段，保证IDC内的网段和VPC内的网段不会重叠！



#### 托管连接的相关限制

- 托管连接对客户侧设备的要求，详见产品概述。
- 托管连接服务仅支持连接到同地域的边界网关，即托管专线和边界网关属于同一地域。
- 使用托管连接前，应规划好京东云托管区内和VPC内的网段，保证京东云托管区内的网段和VPC内的网段不会重叠！



#### 私有网络相关资源配额

| 资源	| 限制	| 例外申请方式	|
| :-: | :-: | :-: |
|同地域物理连接+托管专线数	|10	| 工单	|
|每个物理连接上创建的专线通道数	|50	| 工单	|
|每个托管专线上创建的托管通道数	|50	| 工单	|
|同地域边界网关数	|1	| 工单	|
|同一边界网关的路由规则数	|50	| 工单	|

