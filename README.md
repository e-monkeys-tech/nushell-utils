# Nushell useful snippets

## Build project with rust toolchain
```bash
git clone https://github.com/pbackz/nushell-utils
cargo build --release
```

## Use docker image 
```bash
docker run -it docker.io/pbackz/nushell-utils:latest

Welcome to Nushell 0.21.0 (type 'help' for more info)
/opt/nushell-utils(main)>
```

## CLI functions usage
```nu
> find_files_acceeded_since! . .nu 1wk
───┬─────────────────────────────────────────────────────
 0 │ nushell-az-functions/az_functions.nu|28 mins ago    
 1 │ nushell-odds-api-client/odds-api-ctl.nu|14 mins ago 
 2 │ nushell-utils/utils_functions.nu|37 mins ago        
───┴─────────────────────────────────────────────────────

❯ find_files_modified_since! swift-client-rs/ .rs 1day
───┬──────────────────────────────────────────────────────────────────────────────────────────────────────────
 0 │ swift-client-rs/examples/list-containers.rs|9 hours ago                                                  
 1 │ swift-client-rs/src/main.rs|9 hours ago                                                                  
 2 │ swift-client-rs/target/release/build/mime_guess-b81b2db6ddcf2995/out/mime_types_generated.rs|9 hours ago 
 3 │ swift-client-rs/target/release/build/proc-macro-nested-c460b5ad1c5b68bc/out/count.rs|9 hours ago         
───┴──────────────────────────────────────────────────────────────────────────────────────────────────────────
```