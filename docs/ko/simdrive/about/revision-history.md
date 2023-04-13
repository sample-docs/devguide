# Revision History
This section describes the revision history of the document in chronological order.

---
<br>

| Document Version | Product Version | Release Date  | Descriptions             | Author  |
| :--------------- | :---------------| :------------ | :----------------------- | :------ |
| 1.0              | Alpha 1.0            | April 4, 2023   | Initial Release   | MORAI Engineering Service Team |


|  Version        | Release Date | Additions and Changes   | Bug Fixes   | 
| --------------- | :----------- | ----------------------- | ----------- |
|  Alpha 1.0      | 2023/03/27   | Initial distribution    |             | 




[`tags_extra_files`](#+tags.tags_extra_files){ #+tags.tags_extra_files }

:   [:octicons-tag-24: insiders-4.20.0][Insiders] · :octicons-milestone-24: 
    Default: _none_ – This option specifies additional pages, i.e. to render
    subsets of the [tags index], in order to provide scoped tags indexes for 
    specific sections:

    ``` yaml
    plugins:
      - tags:
          tags_extra_files:
            compatibility.md:
              - compat # (1)!
            web.md:
              - html
              - js
              - css
    ```

    1.  Each page can be assigned a list of [tag identifiers], which must be
        defined as part of `extra.tags` in `mkdocs.yml`:

        ``` yaml
        extra:
          tags:
            Compatibility: compat
            HTML5: html
            JavaScript: js
            CSS: css
        ```

        In this example, all pages with the tag `Compatibility` will be included 
        in the additional tags index on `compatibility.md`, all pages defining
        at least one of the tags `HTML5`, `JavaScript` or `CSS` will be included
        in the additional tags index on `web.md`.
