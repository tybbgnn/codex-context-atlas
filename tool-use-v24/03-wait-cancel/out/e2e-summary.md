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
    "action_count": 9,
    "bb_covered": 235,
    "bb_total": 235,
    "execution_node_count": 20,
    "goal_count": 3,
    "message_count": 11,
    "phase_count": 3
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
      "source_line": "core/src/tools/parallel.rs:250 (macro)"
    },
    {
      "callee": "<std::result::Result<tools::registry::AnyToolResult, codex_tools::FunctionCallError> as std::ops::FromResidual<std::result::Result<std::convert::Infallible, codex_tools::FunctionCallError>>>::from_residual",
      "category": "declaration",
      "def_path_hash": "006f519113f498ad2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:253 (macro)"
    },
    {
      "callee": "std::option::Option::<tools::parallel::ToolCallTimingGuard>::as_mut",
      "category": "declaration",
      "def_path_hash": "0403f53630f0138e2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:286"
    },
    {
      "callee": "<tracing::Level as std::cmp::PartialOrd<tracing::level_filters::LevelFilter>>::le",
      "category": "declaration",
      "def_path_hash": "05ddace4dddbaf572bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:2807"
    },
    {
      "callee": "core::f32::<impl f32>::max",
      "category": "declaration",
      "def_path_hash": "06934992ac36a48e2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:255"
    },
    {
      "callee": "tracing::Metadata::<'_>::fields",
      "category": "declaration",
      "def_path_hash": "0a622101c76a53bb5f065356c969b0a0",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:697"
    },
    {
      "callee": "core::panicking::panic_fmt",
      "category": "declaration",
      "def_path_hash": "0d96ec32223158742bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.rustup/toolchains/nightly-2026-03-01-aarch64-apple-darwin/lib/rustlib/src/rust/library/core/src/panic.rs:62 (macro)"
    },
    {
      "callee": "std::future::poll_fn::<tools::parallel::ToolCallRuntime::handle_tool_call_with_source::{closure#2}::__tokio_select_util::Out<std::result::Result<std::result::Result<tools::registry::AnyToolResult, codex_tools::FunctionCallError>, tokio::task::JoinError>, ()>, {closure@$CARGO_HOME/registry/src/index.crates.io-1949cf8c6b5b557f/tokio-1.52.3/src/macros/select.rs:659:46: 659:50}>",
      "category": "declaration",
      "def_path_hash": "10c47609f83f24852bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tokio-1.52.3/src/macros/select.rs:659 (macro)"
    },
    {
      "callee": "std::option::Option::<&str>::filter::<{closure@core/src/tools/call_trace.rs:86:17: 86:28}>",
      "category": "declaration",
      "def_path_hash": "151b2739ff3556ae2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/call_trace.rs:83"
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
      "callee": "std::fmt::Arguments::<'_>::from_str_nonconst",
      "category": "declaration",
      "def_path_hash": "19819a7ed67a09972bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.rustup/toolchains/nightly-2026-03-01-aarch64-apple-darwin/lib/rustlib/src/rust/library/core/src/panic.rs:62 (macro)"
    },
    {
      "callee": "tokio_util::sync::CancellationToken::cancelled",
      "category": "declaration",
      "def_path_hash": "1b8c95ccfe50c9f338787ccc291f4d48",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:251"
    },
    {
      "callee": "tokio_util::task::AbortOnDropHandle::<std::result::Result<tools::registry::AnyToolResult, codex_tools::FunctionCallError>>::abort",
      "category": "declaration",
      "def_path_hash": "231cdd22fa667c8338787ccc291f4d48",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:257"
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
      "callee": "<u8 as std::default::Default>::default",
      "category": "declaration",
      "def_path_hash": "398b07c59b8554412bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tokio-1.52.3/src/macros/select.rs:622 (macro)"
    },
    {
      "callee": "<std::sync::Arc<session::session::Session> as std::convert::AsRef<session::session::Session>>::as_ref",
      "category": "declaration",
      "def_path_hash": "39d972858970f2b32bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:270"
    },
    {
      "callee": "<std::sync::Arc<session::turn_context::TurnContext> as std::convert::AsRef<session::turn_context::TurnContext>>::as_ref",
      "category": "declaration",
      "def_path_hash": "39d972858970f2b32bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:271"
    },
    {
      "callee": "tokio::task::JoinError::is_cancelled",
      "category": "declaration",
      "def_path_hash": "498f9847f89ff8fc714909b4a5023950",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:260"
    },
    {
      "callee": "std::pin::Pin::<&mut std::future::PollFn<{closure@$CARGO_HOME/registry/src/index.crates.io-1949cf8c6b5b557f/tokio-1.52.3/src/macros/select.rs:659:46: 659:50}>>::new_unchecked",
      "category": "declaration",
      "def_path_hash": "57dad189d36364332bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tokio-1.52.3/src/macros/select.rs:741 (macro)"
    },
    {
      "callee": "std::pin::Pin::<&mut tokio_util::task::AbortOnDropHandle<std::result::Result<tools::registry::AnyToolResult, codex_tools::FunctionCallError>>>::new_unchecked",
      "category": "declaration",
      "def_path_hash": "57dad189d36364332bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:253 (macro)"
    },
    {
      "callee": "std::pin::Pin::<&mut tokio_util::task::AbortOnDropHandle<std::result::Result<tools::registry::AnyToolResult, codex_tools::FunctionCallError>>>::new_unchecked",
      "category": "declaration",
      "def_path_hash": "57dad189d36364332bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:258 (macro)"
    },
    {
      "callee": "std::pin::Pin::<&mut {async fn body of tools::lifecycle::notify_tool_aborted()}>::new_unchecked",
      "category": "declaration",
      "def_path_hash": "57dad189d36364332bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:276 (macro)"
    },
    {
      "callee": "<std::future::PollFn<{closure@$CARGO_HOME/registry/src/index.crates.io-1949cf8c6b5b557f/tokio-1.52.3/src/macros/select.rs:659:46: 659:50}> as futures::Future>::poll",
      "category": "declaration",
      "def_path_hash": "591fc3e935af0c362bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tokio-1.52.3/src/macros/select.rs:741 (macro)"
    },
    {
      "callee": "<tokio_util::task::AbortOnDropHandle<std::result::Result<tools::registry::AnyToolResult, codex_tools::FunctionCallError>> as futures::Future>::poll",
      "category": "declaration",
      "def_path_hash": "591fc3e935af0c362bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:253 (macro)"
    },
    {
      "callee": "<tokio_util::task::AbortOnDropHandle<std::result::Result<tools::registry::AnyToolResult, codex_tools::FunctionCallError>> as futures::Future>::poll",
      "category": "declaration",
      "def_path_hash": "591fc3e935af0c362bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:258 (macro)"
    },
    {
      "callee": "<{async fn body of tools::lifecycle::notify_tool_aborted()} as futures::Future>::poll",
      "category": "declaration",
      "def_path_hash": "591fc3e935af0c362bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:276 (macro)"
    },
    {
      "callee": "tracing::callsite::DefaultCallsite::interest",
      "category": "declaration",
      "def_path_hash": "6141864431f3336c5f065356c969b0a0",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:681"
    },
    {
      "callee": "std::fmt::Arguments::<'_>::new::<32, 1>",
      "category": "declaration",
      "def_path_hash": "6488302cb95ba4ee2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.rustup/toolchains/nightly-2026-03-01-aarch64-apple-darwin/lib/rustlib/src/rust/library/alloc/src/macros.rs:114"
    },
    {
      "callee": "std::hint::must_use::<std::string::String>",
      "category": "declaration",
      "def_path_hash": "7502e9a8aa1e55562bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.rustup/toolchains/nightly-2026-03-01-aarch64-apple-darwin/lib/rustlib/src/rust/library/alloc/src/macros.rs:113"
    },
    {
      "callee": "tracing::Span::record::<str, bool>",
      "category": "declaration",
      "def_path_hash": "80a383e03dd8ea70417ad177881c8bc3",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:256"
    },
    {
      "callee": "<tracing::callsite::DefaultCallsite as tracing::Callsite>::metadata",
      "category": "declaration",
      "def_path_hash": "8134ffbf34a2a9aa5f065356c969b0a0",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:682"
    },
    {
      "callee": "core::fmt::rt::Argument::<'_>::new_debug::<tokio::task::JoinError>",
      "category": "declaration",
      "def_path_hash": "8c6f307cc2d7a5c32bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:300"
    },
    {
      "callee": "std::sync::atomic::AtomicBool::load",
      "category": "declaration",
      "def_path_hash": "9e0693cd4d13dfc32bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:252"
    },
    {
      "callee": "std::result::Result::<std::result::Result<tools::registry::AnyToolResult, codex_tools::FunctionCallError>, tokio::task::JoinError>::map_err::<codex_tools::FunctionCallError, fn(tokio::task::JoinError) -> codex_tools::FunctionCallError {tools::parallel::ToolCallRuntime::tool_task_join_error}>",
      "category": "declaration",
      "def_path_hash": "b208b59e6d19ae672bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:250"
    },
    {
      "callee": "std::result::Result::<std::result::Result<tools::registry::AnyToolResult, codex_tools::FunctionCallError>, tokio::task::JoinError>::map_err::<codex_tools::FunctionCallError, fn(tokio::task::JoinError) -> codex_tools::FunctionCallError {tools::parallel::ToolCallRuntime::tool_task_join_error}>",
      "category": "declaration",
      "def_path_hash": "b208b59e6d19ae672bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:253"
    },
    {
      "callee": "std::fmt::format",
      "category": "declaration",
      "def_path_hash": "b4651e06de7cdf100881b6f26f9b543c",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.rustup/toolchains/nightly-2026-03-01-aarch64-apple-darwin/lib/rustlib/src/rust/library/alloc/src/macros.rs:114"
    },
    {
      "callee": "tracing::field::display::<&codex_protocol::ThreadId>",
      "category": "declaration",
      "def_path_hash": "b9118929da094bd45f065356c969b0a0",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:2836"
    },
    {
      "callee": "std::time::Instant::elapsed",
      "category": "declaration",
      "def_path_hash": "c3dabd15f461f5e07e6be08242084ac8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:255"
    },
    {
      "callee": "std::string::String::as_str",
      "category": "declaration",
      "def_path_hash": "c5047a448ff30a9f0881b6f26f9b543c",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/call_trace.rs:76"
    },
    {
      "callee": "std::string::String::as_str",
      "category": "declaration",
      "def_path_hash": "c5047a448ff30a9f0881b6f26f9b543c",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:272"
    },
    {
      "callee": "<std::result::Result<std::result::Result<tools::registry::AnyToolResult, codex_tools::FunctionCallError>, codex_tools::FunctionCallError> as std::ops::Try>::branch",
      "category": "declaration",
      "def_path_hash": "c554288a6d26ad412bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:250 (macro)"
    },
    {
      "callee": "<std::result::Result<std::result::Result<tools::registry::AnyToolResult, codex_tools::FunctionCallError>, codex_tools::FunctionCallError> as std::ops::Try>::branch",
      "category": "declaration",
      "def_path_hash": "c554288a6d26ad412bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:253 (macro)"
    },
    {
      "callee": "std::time::Duration::as_secs_f32",
      "category": "declaration",
      "def_path_hash": "cd68882a43d373482bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:255"
    },
    {
      "callee": "<&mut tokio_util::task::AbortOnDropHandle<std::result::Result<tools::registry::AnyToolResult, codex_tools::FunctionCallError>> as std::future::IntoFuture>::into_future",
      "category": "declaration",
      "def_path_hash": "d568101b07447f112bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tokio-1.52.3/src/macros/select.rs:649 (macro)"
    },
    {
      "callee": "<std::future::PollFn<{closure@$CARGO_HOME/registry/src/index.crates.io-1949cf8c6b5b557f/tokio-1.52.3/src/macros/select.rs:659:46: 659:50}> as std::future::IntoFuture>::into_future",
      "category": "declaration",
      "def_path_hash": "d568101b07447f112bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tokio-1.52.3/src/macros/select.rs:741 (macro)"
    },
    {
      "callee": "<tokio_util::sync::WaitForCancellationFuture<'_> as std::future::IntoFuture>::into_future",
      "category": "declaration",
      "def_path_hash": "d568101b07447f112bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tokio-1.52.3/src/macros/select.rs:649 (macro)"
    },
    {
      "callee": "<tokio_util::task::AbortOnDropHandle<std::result::Result<tools::registry::AnyToolResult, codex_tools::FunctionCallError>> as std::future::IntoFuture>::into_future",
      "category": "declaration",
      "def_path_hash": "d568101b07447f112bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:253 (macro)"
    },
    {
      "callee": "<tokio_util::task::AbortOnDropHandle<std::result::Result<tools::registry::AnyToolResult, codex_tools::FunctionCallError>> as std::future::IntoFuture>::into_future",
      "category": "declaration",
      "def_path_hash": "d568101b07447f112bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:258 (macro)"
    },
    {
      "callee": "<{async fn body of tools::lifecycle::notify_tool_aborted()} as std::future::IntoFuture>::into_future",
      "category": "declaration",
      "def_path_hash": "d568101b07447f112bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:276 (macro)"
    },
    {
      "callee": "tokio_util::task::AbortOnDropHandle::<std::result::Result<tools::registry::AnyToolResult, codex_tools::FunctionCallError>>::is_finished",
      "category": "declaration",
      "def_path_hash": "d690d340db7aab6c38787ccc291f4d48",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:252"
    },
    {
      "callee": "std::fmt::Arguments::<'_>::from_str",
      "category": "declaration",
      "def_path_hash": "e02afc86e65edd152bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.rustup/toolchains/nightly-2026-03-01-aarch64-apple-darwin/lib/rustlib/src/rust/library/core/src/panic.rs:62 (macro)"
    },
    {
      "callee": "<std::string::String as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:332"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:264"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:266"
    },
    {
      "callee": "<std::sync::Arc<session::turn_context::TurnContext> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:264"
    },
    {
      "callee": "<std::sync::Arc<tools::context::ToolCallState> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:252"
    },
    {
      "callee": "<dyn codex_tools::ToolOutput as codex_tools::ToolOutput>::set_handler_duration_ms",
      "category": "declaration",
      "def_path_hash": "fe1745fcc7cc8e5db95c18fb6b5909c0",
      "reason": "dynamic dispatch has no concrete body",
      "source_line": "core/src/tools/parallel.rs:290"
    }
  ]
}
```
