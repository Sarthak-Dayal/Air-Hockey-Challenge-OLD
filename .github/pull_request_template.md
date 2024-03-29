## Description
<!--- Provide a general summary of your changes in here-->

## Types of changes
<!--- What types of changes does your code introduce? Put an `x` in all the boxes that apply: -->
- [ ] Bug fix
- [ ] New feature
- [ ] New algorithm
- [ ] Documentation

## Checklist:
<!--- Go over all the following points, and put an `x` in all the boxes that apply. -->
<!--- If you're unsure about any of these, don't hesitate to ask. We're here to help! -->
- [ ] I've read the [CONTRIBUTION](https://docs.cleanrl.dev/contribution/) guide (**required**).
- [ ] I have ensured `pre-commit run --all-files` passes (**required**).
- [ ] I have updated the tests accordingly (if applicable).
- [ ] I have updated the documentation and previewed the changes via `mkdocs serve`.
    - [ ] I have explained note-worthy implementation details.
    - [ ] I have explained the logged metrics.
    - [ ] I have added links to the original paper and related papers.

If you need to run benchmark experiments for a performance-impacting changes:

- [ ] I have contacted @vwxyzjn to obtain access to the [openrlbenchmark W&B team](https://wandb.ai/openrlbenchmark).
- [ ] I have used the [benchmark utility](/get-started/benchmark-utility/) to submit the tracked experiments to the [openrlbenchmark/cleanrl](https://wandb.ai/openrlbenchmark/cleanrl) W&B project, optionally with `--capture_video`.
- [ ] I have performed RLops with `python -m openrlbenchmark.rlops`.
    - For new feature or bug fix:
        - [ ] I have used the RLops utility to understand the performance impact of the changes and confirmed there is no regression.
    - For new algorithm:
        - [ ] I have created a table comparing my results against those from reputable sources (i.e., the original paper or other reference implementation).
    - [ ] I have added the learning curves generated by the `python -m openrlbenchmark.rlops` utility to the documentation.
    - [ ] I have added links to the tracked experiments in W&B, generated by `python -m openrlbenchmark.rlops ....your_args... --report`,  to the documentation.

