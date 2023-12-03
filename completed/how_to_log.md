# How to Log

## Module description

In this module, we will learn how to log in ndnSIM.

There are multiple ways to log in ndnSIM. We will discuss them one by one.

## Procedure

### 1. Using `NS_LOG`

`NS_LOG` is a macro defined in `ns3/log.h` file. It is used to log in ndnSIM. It is used as follows:

```cpp 
NS_LOG_INFO("Some information");

NS_LOG_DEBUG("Some debug information");

NS_LOG_WARN("Some warning");

NS_LOG_ERROR("Some error");
```

### 2. Using `NS_LOG_COMPONENT_DEFINE`

`NS_LOG_COMPONENT_DEFINE` is a macro defined in `ns3/log.h` file. It is used to log in ndnSIM. It is used as follows:

```cpp
NS_LOG_COMPONENT_DEFINE("Some component");

NS_LOG_INFO("Some information");

NS_LOG_DEBUG("Some debug information");

NS_LOG_WARN("Some warning");

NS_LOG_ERROR("Some error");
```

To see the logs, you need to set the log level of the component. It can be done as follows:

```cpp
LogComponentEnable("Some component", LOG_LEVEL);

NS_LOG="<Component name>:<Log level>" ./waf --run <program name>
```

We can use `grep` in linux to filter the logs. For example, if we want to see only the `INFO` logs, we can use the following command:

```cpp
NS_LOG="Some component:*" ./waf --run <program name> | grep "INFO"
```