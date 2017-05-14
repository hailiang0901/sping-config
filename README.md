# hfconfigserver

## 配置文件组织层次:
- search-api ---------------->项目名称
- |- dev    ---------------->开发环境
- ----|-cache.properties
- ----|-application.properties
- |- ci     ---------------->CI环境
- ----|-cache.properties
- ----|-application.properties
- |- st     ---------------->St环境
- ----|-cache.properties
- ----|-application.properties
- |- anhouse     ----------->anhouse环境
- ----|-cache.properties
- ----|-application.properties
- |- ga     ---------------->ga环境
- ----|-cache.properties
- ----|-application.properties
- 
- hdmp-api ---------------->项目名称
- |- dev    ---------------->开发环境
- |- ci     ---------------->CI环境
- |- st     ---------------->St环境
- |- anhouse     ----------->anhouse环境
- |- ga     ---------------->ga环境

## 配置文件访问
http://configserver.iop.com/api/v1//{appName}/{profile}/{configName}.{suffix}

- 如search-api工程 application.properties配置文件：
1. dev环境： http://configserver.iop.com/api/v1/search-api/dev/application.properties
2. st环境： http://configserver.iop.com/api/v1/search-api/st/application.properties
