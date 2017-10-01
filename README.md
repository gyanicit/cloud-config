# cloud-config 
# Git by default looks for application.property but we can specify search paths
spring:
  cloud:
    config:
      server:
        git:
          uri: https://github.com/gyanicit/cloud-config
          #username: <username of git repository in case of private repository>
          #password: <password of git repository in case of private repository>
          search-paths:
          - app* #patter search support is available 
          # - app1,app2  #For Exact matching

