This is UncaughtExceptionHandler subclass, you can catch exceptions that you do not handle.

You can initialization in  application : 
GlobalCrashHelper.getInstance().init(this);

You can also use other initialization method initialization in  application：
public void init(@NonNull Context context, @NonNull String catch_log_path)；
public void init(@NonNull Context context, @NonNull String catch_log_path, @NonNull String exception_prompt_info)；
public void init(@NonNull Context context, @NonNull String catch_log_path, @NonNull String exception_prompt_info,@Nullable QuitCallback onExceptionCollectionComplete)
