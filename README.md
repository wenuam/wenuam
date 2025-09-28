# wenuam

Meaningful development studio with a mindset.

Software architecture, project management, embedded system.

* Home

https://github.com/wenuam

## Repositories

```mermaid
%%{init: {'theme': 'forest'}}%%
flowchart TD
	subgraph wm[wm]
		subgraph wm_app[app]
			subgraph wm_app_doc[doc]
				subgraph wm_app_doc_gen[gen]
					wm_app_doc_gen_latex[latex]
				end
				subgraph wm_app_doc_wiki[wiki]
					subgraph wm_app_doc_wiki_tiddly[tiddly]
						wm_app_doc_wiki_tiddly__bob[bob]
					end
				end
			end
			subgraph wm_app_dev[dev]
				subgraph wm_app_dev_lng[lng]
					wm_app_dev_lng_python[python]
				end
			end
		end
		subgraph wm_dev[dev]
			direction LR
			subgraph wm_dev_lng[lng]
				subgraph wm_dev_lng_c[c]
					wm_dev_lng_c_includes[includes]
				end
				wm_dev_lng_fori[fori]
			end
			subgraph wm_dev_scm[scm]
				subgraph wm_dev_scm_git[git]
					wm_dev_scm_git_helpers[helpers]
				end
			end
		end
		subgraph wm_key[key]
			direction LR
			subgraph wm_key_map[map]
				wm_key_map_cfilorux[cfilorux]
			end
		end
	end

	click wm "https://github.com/wenuam" _blank

	click wm_app "https://github.com/wenuam/wm_app" _blank
	click wm_app_doc "https://github.com/wenuam/wm_app_doc" _blank
		click wm_app_doc_gen "https://github.com/wenuam/wm_app_doc_gen" _blank
			click wm_app_doc_gen_latex "https://github.com/wenuam/wm_app_doc_gen_latex" _blank
		click wm_app_doc_wiki "https://github.com/wenuam/wm_app_doc_wiki" _blank
			click wm_app_doc_wiki_tiddly "https://github.com/wenuam/wm_app_doc_wiki_tiddly" _blank
				click wm_app_doc_wiki_tiddly__bob "https://github.com/wenuam/wm_app_doc_wiki_tiddly__bob" _blank
	click wm_app_lng "https://github.com/wenuam/wm_app_dev" _blank
		click wm_app_dev_lng "https://github.com/wenuam/wm_app_dev_lng" _blank
			click wm_app_dev_lng_python "https://github.com/wenuam/wm_app_dev_lng_python" _blank

	click wm_dev "https://github.com/wenuam/wm_dev" _blank
	click wm_dev_lng "https://github.com/wenuam/wm_dev_lng" _blank
		click wm_dev_lng_c "https://github.com/wenuam/wm_dev_lng_c" _blank
			click wm_dev_lng_c_includes "https://github.com/wenuam/wm_dev_lng_c_includes" _blank
		click wm_dev_lng_fori "https://github.com/wenuam/wm_dev_lng_fori" _blank
	click wm_dev_scm "https://github.com/wenuam/wm_dev_scm" _blank
		click wm_dev_scm_git "https://github.com/wenuam/wm_dev_scm_git" _blank
			click wm_dev_scm_git_helpers "https://github.com/wenuam/wm_dev_scm_git_helpers" _blank

	click wm_key "https://github.com/wenuam/wm_key" _blank
		click wm_key_map "https://github.com/wenuam/wm_key_map" _blank
			click wm_key_map_cfilorux "https://github.com/wenuam/wm_key_map_cfilorux" _blank

	classDef lvl0 fill:#fc9,stroke:#da7;
	classDef lvl1 fill:#eb8,stroke:#c96;
	classDef lvl2 fill:#da7,stroke:#b85;
	classDef lvl3 fill:#c96,stroke:#a74;
	classDef lvl4 fill:#b85,stroke:#963;
	classDef lvl5 fill:#a74,stroke:#852;

%%	style wm fill:#f66
	class wm lvl0;

	class wm_app lvl1

	class wm_app_doc lvl2
	class wm_app_doc_gen lvl3
	class wm_app_doc_gen_latex lvl4
	class wm_app_doc_wiki lvl3
	class wm_app_doc_wiki_tiddly lvl4
	class wm_app_doc_wiki_tiddly__bob lvl5

	class wm_app_dev lvl2
	class wm_app_dev_lng lvl3
	class wm_app_dev_lng_python lvl4

	class wm_dev lvl1
	class wm_dev_lng lvl2
	class wm_dev_lng_c lvl3
	class wm_dev_lng_c_includes lvl4

	class wm_dev_lng_fori lvl3

	class wm_dev_scm lvl2
	class wm_dev_scm_git lvl3
	class wm_dev_scm_git_helpers lvl4

	class wm_key lvl1
	class wm_key_map lvl2
	class wm_key_map_cfilorux lvl3
```

The naming convention is from general to specific :

```wm_key_name(__impl)```

* wm : wenuam's compact form
* key : bi/tri-grams for the section (see `Keys` section below)
* name : repository name or subsection (may be like `key`)
* __impl : specific implementation (optional)

Some repositories may be used in another as submodule, often using only their `name` with no prefix.

Such repositories may not keep a complete history and old binaries be scrubbed, pulling must be forced.

### Keys

Repository keys are as follow (non exhaustive) :

Lower case to prevent disparity/conflict. When in UPPER CASE it signifies a GROUP.

<details>
<summary>Keys (click to expand)</summary>
<p>

| key	| Explanation						|
| :---	| :---								|
| app	| Applications, portable or not		|
| cer	| Certificat						|
| cnv	| Converter							|
| com	| Communication buses				|
| dat	| Data								|
| db	| Database							|
| dev	| Development tools and libraries	|
| doc	| Documentation						|
| ed	| Editor							|
| emu	| Emulation							|
| gen	| Generator							|
| img	| Image (format, viewer, editor)	|
| key	| Keyboard (layout, mapping)		|
| lng	| Languages (programming, natural)	|
| map	| Mapping							|
| net	| Network (protocols, stacks)		|
| os	| Operating system					|
| pcb	| Electronic and related			|
| prj	| Project (files, methodology)		|
| scm	| Source Code Management			|
| snd	| Sound	(format, player, editor)	|
| sys	| System							|
| txt	| Text								|
| ui	| User interface (graphic, text)	|
| utl	| Utility							|
| vid	| Video (format, player, editor)	|
| web	| Internet (format, berowser)		|

</p>
</details>
