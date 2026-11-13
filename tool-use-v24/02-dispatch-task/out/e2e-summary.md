# 验收结果

passed

MIR：clean

全部必需检查已通过，主 body BB 全覆盖。公开报告省略本机命令与日志路径。

```json
{
  "status": "passed",
  "passed": true,
  "clean_pass": true,
  "mir_status": "clean",
  "missing_mir_count": 0,
  "counts": {
    "action_count": 7,
    "bb_covered": 202,
    "bb_total": 202,
    "execution_node_count": 16,
    "goal_count": 3,
    "message_count": 7,
    "phase_count": 2
  },
  "browser_checked": true,
  "checks_not_run": [],
  "checks": {
    "batch": {
      "passed": true
    },
    "batch-reference": {
      "passed": true
    },
    "browser": {
      "passed": true
    },
    "contract": {
      "passed": true
    },
    "duplicates": {
      "passed": true
    },
    "hard-rules": {
      "passed": true
    },
    "independent-source": {
      "passed": true
    },
    "principles": {
      "passed": true
    },
    "regressions": {
      "passed": true
    }
  },
  "source_commit": "c248f6d48b97eb4a2aa56147a0b11b7d763278b9",
  "registered_deviation_count": 0,
  "missing_mir": [
    {
      "callee": "<std::result::Result<tools::registry::AnyToolResult, codex_tools::FunctionCallError> as std::ops::FromResidual<std::result::Result<std::convert::Infallible, codex_tools::FunctionCallError>>>::from_residual",
      "category": "declaration",
      "def_path_hash": "006f519113f498ad2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:198 (macro)"
    },
    {
      "callee": "<tracing::Level as std::cmp::PartialOrd<tracing::level_filters::LevelFilter>>::le",
      "category": "declaration",
      "def_path_hash": "05ddace4dddbaf572bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:2807"
    },
    {
      "callee": "tracing::Metadata::<'_>::fields",
      "category": "declaration",
      "def_path_hash": "0a622101c76a53bb5f065356c969b0a0",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:697"
    },
    {
      "callee": "std::option::Option::<&str>::filter::<{closure@core/src/tools/call_trace.rs:86:17: 86:28}>",
      "category": "declaration",
      "def_path_hash": "151b2739ff3556ae2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/call_trace.rs:83"
    },
    {
      "callee": "std::mem::drop::<tokio_util::either::Either<tokio::sync::RwLockReadGuard<'_, ()>, tokio::sync::RwLockWriteGuard<'_, ()>>>",
      "category": "declaration",
      "def_path_hash": "155d8318ccbc4b342bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:228"
    },
    {
      "callee": "tracing::__macro_support::__is_enabled",
      "category": "declaration",
      "def_path_hash": "181afd5c325c6bab417ad177881c8bc3",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:682"
    },
    {
      "callee": "std::option::Option::<std::string::String>::as_deref",
      "category": "declaration",
      "def_path_hash": "1835c87e5e8cca882bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/call_trace.rs:83"
    },
    {
      "callee": "tracing::subscriber::Interest::is_never",
      "category": "declaration",
      "def_path_hash": "266ce036cd642c235f065356c969b0a0",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:682"
    },
    {
      "callee": "tracing::level_filters::LevelFilter::current",
      "category": "declaration",
      "def_path_hash": "2cc74db53adc0c125f065356c969b0a0",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:2808"
    },
    {
      "callee": "std::sync::OnceLock::<std::time::Instant>::set",
      "category": "declaration",
      "def_path_hash": "48cc4f1a642ba3427e6be08242084ac8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:213"
    },
    {
      "callee": "std::pin::Pin::<&mut std::pin::Pin<std::boxed::Box<dyn futures::Future<Output = ()> + std::marker::Send>>>::new_unchecked",
      "category": "declaration",
      "def_path_hash": "57dad189d36364332bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:202 (macro)"
    },
    {
      "callee": "std::pin::Pin::<&mut tracing::instrument::Instrumented<{async fn body of tools::router::ToolRouter::dispatch_tool_call_with_state()}>>::new_unchecked",
      "category": "declaration",
      "def_path_hash": "57dad189d36364332bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:227 (macro)"
    },
    {
      "callee": "std::pin::Pin::<&mut {async fn body of tokio::sync::RwLock<()>::read()}>::new_unchecked",
      "category": "declaration",
      "def_path_hash": "57dad189d36364332bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:206 (macro)"
    },
    {
      "callee": "std::pin::Pin::<&mut {async fn body of tokio::sync::RwLock<()>::write()}>::new_unchecked",
      "category": "declaration",
      "def_path_hash": "57dad189d36364332bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:208 (macro)"
    },
    {
      "callee": "<std::pin::Pin<std::boxed::Box<dyn futures::Future<Output = ()> + std::marker::Send>> as futures::Future>::poll",
      "category": "declaration",
      "def_path_hash": "591fc3e935af0c362bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:202 (macro)"
    },
    {
      "callee": "<tracing::instrument::Instrumented<{async fn body of tools::router::ToolRouter::dispatch_tool_call_with_state()}> as futures::Future>::poll",
      "category": "declaration",
      "def_path_hash": "591fc3e935af0c362bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:227 (macro)"
    },
    {
      "callee": "<{async fn body of tokio::sync::RwLock<()>::read()} as futures::Future>::poll",
      "category": "declaration",
      "def_path_hash": "591fc3e935af0c362bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:206 (macro)"
    },
    {
      "callee": "<{async fn body of tokio::sync::RwLock<()>::write()} as futures::Future>::poll",
      "category": "declaration",
      "def_path_hash": "591fc3e935af0c362bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:208 (macro)"
    },
    {
      "callee": "tracing::callsite::DefaultCallsite::interest",
      "category": "declaration",
      "def_path_hash": "6141864431f3336c5f065356c969b0a0",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:681"
    },
    {
      "callee": "tokio::sync::RwLock::<()>::read",
      "category": "declaration",
      "def_path_hash": "7ece2014ad00c356714909b4a5023950",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:206"
    },
    {
      "callee": "7f7c8113c0e404b6714909b4a5023950",
      "category": "declaration",
      "def_path_hash": "7f7c8113c0e404b6714909b4a5023950",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "?:None"
    },
    {
      "callee": "<tracing::callsite::DefaultCallsite as tracing::Callsite>::metadata",
      "category": "declaration",
      "def_path_hash": "8134ffbf34a2a9aa5f065356c969b0a0",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:682"
    },
    {
      "callee": "tokio::sync::RwLock::<()>::write",
      "category": "declaration",
      "def_path_hash": "83a71c6f85481ebd714909b4a5023950",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:208"
    },
    {
      "callee": "tracing::field::display::<&codex_protocol::ThreadId>",
      "category": "declaration",
      "def_path_hash": "b9118929da094bd45f065356c969b0a0",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:2836"
    },
    {
      "callee": "<dyn tools::registry::CoreToolRuntime as tools::registry::CoreToolRuntime>::wait_until_ready",
      "category": "declaration",
      "def_path_hash": "c0d1e4ad485880a07f347cbdcc2b778a",
      "reason": "dynamic dispatch has no concrete body",
      "source_line": "core/src/tools/parallel.rs:200"
    },
    {
      "callee": "std::string::String::as_str",
      "category": "declaration",
      "def_path_hash": "c5047a448ff30a9f0881b6f26f9b543c",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/call_trace.rs:76"
    },
    {
      "callee": "<std::result::Result<std::option::Option<tokio_util::task::task_tracker::TaskTrackerToken>, codex_tools::FunctionCallError> as std::ops::Try>::branch",
      "category": "declaration",
      "def_path_hash": "c554288a6d26ad412bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:198 (macro)"
    },
    {
      "callee": "std::time::Instant::now",
      "category": "declaration",
      "def_path_hash": "c9a699096f0df9507e6be08242084ac8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:213"
    },
    {
      "callee": "<{async fn body of tools::router::ToolRouter::dispatch_tool_call_with_state()} as tracing::Instrument>::instrument",
      "category": "declaration",
      "def_path_hash": "cd825715b398554f417ad177881c8bc3",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:216"
    },
    {
      "callee": "<std::pin::Pin<std::boxed::Box<dyn futures::Future<Output = ()> + std::marker::Send>> as std::future::IntoFuture>::into_future",
      "category": "declaration",
      "def_path_hash": "d568101b07447f112bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:202 (macro)"
    },
    {
      "callee": "<tracing::instrument::Instrumented<{async fn body of tools::router::ToolRouter::dispatch_tool_call_with_state()}> as std::future::IntoFuture>::into_future",
      "category": "declaration",
      "def_path_hash": "d568101b07447f112bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:227 (macro)"
    },
    {
      "callee": "<{async fn body of tokio::sync::RwLock<()>::read()} as std::future::IntoFuture>::into_future",
      "category": "declaration",
      "def_path_hash": "d568101b07447f112bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:206 (macro)"
    },
    {
      "callee": "<{async fn body of tokio::sync::RwLock<()>::write()} as std::future::IntoFuture>::into_future",
      "category": "declaration",
      "def_path_hash": "d568101b07447f112bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:208 (macro)"
    },
    {
      "callee": "<tracing::Span as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:226"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:236"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:238"
    },
    {
      "callee": "<std::sync::Arc<dyn tools::registry::CoreToolRuntime> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:200"
    },
    {
      "callee": "<std::sync::Arc<session::turn_context::TurnContext> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:236"
    },
    {
      "callee": "<std::sync::Arc<std::sync::OnceLock<std::time::Instant>> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:213"
    },
    {
      "callee": "<std::sync::Arc<tokio::sync::RwLock<()>> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:206"
    },
    {
      "callee": "<std::sync::Arc<tokio::sync::RwLock<()>> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:208"
    },
    {
      "callee": "<std::sync::Arc<tools::router::ToolRouter> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:216"
    },
    {
      "callee": "efc7711f594fd0f9714909b4a5023950",
      "category": "declaration",
      "def_path_hash": "efc7711f594fd0f9714909b4a5023950",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "?:None"
    }
  ]
}
```
