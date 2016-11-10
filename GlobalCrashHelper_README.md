#GlobalCrashHelper

This is UncaughtExceptionHandler subclass, you can catch exceptions that you do not handle.

## Getting started

In your `Application` class:

```java
public class ExampleApplication extends Application {

  @Override public void onCreate() {
    super.onCreate();
    GlobalCrashHelper.getInstance().init(this);
  }
}
```
You can also use other initialization method initialization in your `Application` class：

```java
public void init(@NonNull Context context, @NonNull String catch_log_path);

public void init(@NonNull Context context, @NonNull String catch_log_path, @NonNull String exception_prompt_info);

public void init(@NonNull Context context,
                     @NonNull String catch_log_path,
                     @NonNull String exception_prompt_info,
                     @Nullable QuitCallback onExceptionCollectionComplete);
```
