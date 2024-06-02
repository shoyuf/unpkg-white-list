# unpkg-white-list

[![NPM version](https://img.shields.io/npm/v/unpkg-white-list.svg?style=flat-square)](https://npmjs.org/package/unpkg-white-list)
[![CI](https://github.com/cnpm/unpkg-white-list/actions/workflows/nodejs.yml/badge.svg)](https://github.com/cnpm/unpkg-white-list/actions/workflows/nodejs.yml)

[npmmirror.com](https://npmmirror.com) 允许开启 [unpkg 功能](https://www.yuque.com/egg/cnpm/files)的白名单列表，避免 https://x.com/fengmk2/status/1791498406923215020 类似问题

## 添加白名单方式

1、直接在线修改 [package.json](https://github.com/cnpm/unpkg-white-list/edit/master/package.json) 中的 `allowPackages` 字段，
添加你想开启 unpkg 文件同步的 npm 包名和版本号，全量同步版本号可以设置为 `*`。

以同步 [urllib](https://npmmirror.com/package/urllib) 为示例，配置如下：

```json
"allowPackages": {
  ...
  "urllib": {
    "version": "*"
  }
  ...
}
```

当然你发布的是 scoped package，可以直接添加 scope 到白名单 `allowScopes`：

```json
"allowScopes": [
  ...
  "@eggjs",
  ...
]
```

2、修改完成后提交一个 `Pull Request` 合并到 master 分支，等待 Review，合并后会自动发布，预计最长 5 分钟后会全网生效。

## License

[MIT](LICENSE)

<!-- GITCONTRIBUTOR_START -->

## Contributors

|[<img src="https://avatars.githubusercontent.com/u/32174276?v=4" width="100px;"/><br/><sub><b>semantic-release-bot</b></sub>](https://github.com/semantic-release-bot)<br/>|[<img src="https://avatars.githubusercontent.com/u/156269?v=4" width="100px;"/><br/><sub><b>fengmk2</b></sub>](https://github.com/fengmk2)<br/>|[<img src="https://avatars.githubusercontent.com/u/119665355?v=4" width="100px;"/><br/><sub><b>AdingApkgg</b></sub>](https://github.com/AdingApkgg)<br/>|[<img src="https://avatars.githubusercontent.com/u/53730587?v=4" width="100px;"/><br/><sub><b>ChenYFan</b></sub>](https://github.com/ChenYFan)<br/>|[<img src="https://avatars.githubusercontent.com/u/49147660?v=4" width="100px;"/><br/><sub><b>CNFeffery</b></sub>](https://github.com/CNFeffery)<br/>|[<img src="https://avatars.githubusercontent.com/u/9065684?v=4" width="100px;"/><br/><sub><b>SharerMax</b></sub>](https://github.com/SharerMax)<br/>|
| :---: | :---: | :---: | :---: | :---: | :---: |
|[<img src="https://avatars.githubusercontent.com/u/20525492?v=4" width="100px;"/><br/><sub><b>shangzhenyang</b></sub>](https://github.com/shangzhenyang)<br/>|[<img src="https://avatars.githubusercontent.com/u/16996226?v=4" width="100px;"/><br/><sub><b>Ruanxingzhi</b></sub>](https://github.com/Ruanxingzhi)<br/>|[<img src="https://avatars.githubusercontent.com/u/145643935?v=4" width="100px;"/><br/><sub><b>i18n-now</b></sub>](https://github.com/i18n-now)<br/>|[<img src="https://avatars.githubusercontent.com/u/7835220?v=4" width="100px;"/><br/><sub><b>tjyuanpeng</b></sub>](https://github.com/tjyuanpeng)<br/>|[<img src="https://avatars.githubusercontent.com/u/98782978?v=4" width="100px;"/><br/><sub><b>ao-x</b></sub>](https://github.com/ao-x)<br/>|[<img src="https://avatars.githubusercontent.com/u/54071368?v=4" width="100px;"/><br/><sub><b>pig0224</b></sub>](https://github.com/pig0224)<br/>|
|[<img src="https://avatars.githubusercontent.com/u/57941037?v=4" width="100px;"/><br/><sub><b>AIsouler</b></sub>](https://github.com/AIsouler)<br/>|[<img src="https://avatars.githubusercontent.com/u/17870709?v=4" width="100px;"/><br/><sub><b>canisminor1990</b></sub>](https://github.com/canisminor1990)<br/>|[<img src="https://avatars.githubusercontent.com/u/142888681?v=4" width="100px;"/><br/><sub><b>FloatSheep</b></sub>](https://github.com/FloatSheep)<br/>|[<img src="https://avatars.githubusercontent.com/u/1191515?v=4" width="100px;"/><br/><sub><b>ydfzgyj</b></sub>](https://github.com/ydfzgyj)<br/>|[<img src="https://avatars.githubusercontent.com/u/32838658?v=4" width="100px;"/><br/><sub><b>IronKinoko</b></sub>](https://github.com/IronKinoko)<br/>|[<img src="https://avatars.githubusercontent.com/u/50269993?v=4" width="100px;"/><br/><sub><b>jiakun-zhao</b></sub>](https://github.com/jiakun-zhao)<br/>|
|[<img src="https://avatars.githubusercontent.com/u/13492743?v=4" width="100px;"/><br/><sub><b>junlongzzz</b></sub>](https://github.com/junlongzzz)<br/>|[<img src="https://avatars.githubusercontent.com/u/8198408?v=4" width="100px;"/><br/><sub><b>BlackHole1</b></sub>](https://github.com/BlackHole1)<br/>|[<img src="https://avatars.githubusercontent.com/u/8214855?v=4" width="100px;"/><br/><sub><b>zhipenglin</b></sub>](https://github.com/zhipenglin)<br/>|[<img src="https://avatars.githubusercontent.com/u/98106970?v=4" width="100px;"/><br/><sub><b>zypluckyphoenix</b></sub>](https://github.com/zypluckyphoenix)<br/>|[<img src="https://avatars.githubusercontent.com/u/37367461?v=4" width="100px;"/><br/><sub><b>Meetacoo</b></sub>](https://github.com/Meetacoo)<br/>|[<img src="https://avatars.githubusercontent.com/u/22628584?v=4" width="100px;"/><br/><sub><b>Merrg1n</b></sub>](https://github.com/Merrg1n)<br/>|
|[<img src="https://avatars.githubusercontent.com/u/77185868?v=4" width="100px;"/><br/><sub><b>Saammaa</b></sub>](https://github.com/Saammaa)<br/>|[<img src="https://avatars.githubusercontent.com/u/13798931?v=4" width="100px;"/><br/><sub><b>tomgao365</b></sub>](https://github.com/tomgao365)<br/>|[<img src="https://avatars.githubusercontent.com/u/34960995?v=4" width="100px;"/><br/><sub><b>2239559319</b></sub>](https://github.com/2239559319)<br/>|[<img src="https://avatars.githubusercontent.com/u/138312775?v=4" width="100px;"/><br/><sub><b>Xiaovalry</b></sub>](https://github.com/Xiaovalry)<br/>|[<img src="https://avatars.githubusercontent.com/u/119661535?v=4" width="100px;"/><br/><sub><b>Zhizhi-2986</b></sub>](https://github.com/Zhizhi-2986)<br/>|[<img src="https://avatars.githubusercontent.com/u/34203474?v=4" width="100px;"/><br/><sub><b>aoguai</b></sub>](https://github.com/aoguai)<br/>|
|[<img src="https://avatars.githubusercontent.com/u/9837532?v=4" width="100px;"/><br/><sub><b>asdw741111</b></sub>](https://github.com/asdw741111)<br/>|[<img src="https://avatars.githubusercontent.com/u/170389105?v=4" width="100px;"/><br/><sub><b>bukwork</b></sub>](https://github.com/bukwork)<br/>|[<img src="https://avatars.githubusercontent.com/u/47235156?v=4" width="100px;"/><br/><sub><b>cha0sCat</b></sub>](https://github.com/cha0sCat)<br/>|[<img src="https://avatars.githubusercontent.com/u/26962197?v=4" width="100px;"/><br/><sub><b>chilingling</b></sub>](https://github.com/chilingling)<br/>|[<img src="https://avatars.githubusercontent.com/u/55350790?v=4" width="100px;"/><br/><sub><b>dashuaibi45678</b></sub>](https://github.com/dashuaibi45678)<br/>|[<img src="https://avatars.githubusercontent.com/u/22270677?v=4" width="100px;"/><br/><sub><b>fondoger</b></sub>](https://github.com/fondoger)<br/>|
|[<img src="https://avatars.githubusercontent.com/u/160194569?v=4" width="100px;"/><br/><sub><b>ganlinte</b></sub>](https://github.com/ganlinte)<br/>|[<img src="https://avatars.githubusercontent.com/u/122718097?v=4" width="100px;"/><br/><sub><b>gofunn</b></sub>](https://github.com/gofunn)<br/>|[<img src="https://avatars.githubusercontent.com/u/6399899?v=4" width="100px;"/><br/><sub><b>hacke2</b></sub>](https://github.com/hacke2)<br/>|[<img src="https://avatars.githubusercontent.com/u/15273034?v=4" width="100px;"/><br/><sub><b>ikrong</b></sub>](https://github.com/ikrong)<br/>|[<img src="https://avatars.githubusercontent.com/u/118548920?v=4" width="100px;"/><br/><sub><b>kskshaf</b></sub>](https://github.com/kskshaf)<br/>|[<img src="https://avatars.githubusercontent.com/u/54092711?v=4" width="100px;"/><br/><sub><b>lrhtony</b></sub>](https://github.com/lrhtony)<br/>|
|[<img src="https://avatars.githubusercontent.com/u/55302758?v=4" width="100px;"/><br/><sub><b>122cygf</b></sub>](https://github.com/122cygf)<br/>|[<img src="https://avatars.githubusercontent.com/u/14066276?v=4" width="100px;"/><br/><sub><b>mygithub20152015</b></sub>](https://github.com/mygithub20152015)<br/>|[<img src="https://avatars.githubusercontent.com/u/110751236?v=4" width="100px;"/><br/><sub><b>n0127</b></sub>](https://github.com/n0127)<br/>|[<img src="https://avatars.githubusercontent.com/u/73287541?v=4" width="100px;"/><br/><sub><b>ocean-gao</b></sub>](https://github.com/ocean-gao)<br/>|[<img src="https://avatars.githubusercontent.com/u/2926992?v=4" width="100px;"/><br/><sub><b>onlyid</b></sub>](https://github.com/onlyid)<br/>|[<img src="https://avatars.githubusercontent.com/u/9860456?v=4" width="100px;"/><br/><sub><b>poplanchong123</b></sub>](https://github.com/poplanchong123)<br/>|
|[<img src="https://avatars.githubusercontent.com/u/14960340?v=4" width="100px;"/><br/><sub><b>sparkcyf</b></sub>](https://github.com/sparkcyf)<br/>|[<img src="https://avatars.githubusercontent.com/u/997812?v=4" width="100px;"/><br/><sub><b>ssddi456</b></sub>](https://github.com/ssddi456)<br/>|[<img src="https://avatars.githubusercontent.com/u/6936358?v=4" width="100px;"/><br/><sub><b>Yuliang-Lee</b></sub>](https://github.com/Yuliang-Lee)<br/>|[<img src="https://avatars.githubusercontent.com/u/142392685?v=4" width="100px;"/><br/><sub><b>zsj9705</b></sub>](https://github.com/zsj9705)<br/>|[<img src="https://avatars.githubusercontent.com/u/38517192?v=4" width="100px;"/><br/><sub><b>lisonge</b></sub>](https://github.com/lisonge)<br/>|[<img src="https://avatars.githubusercontent.com/u/29626873?v=4" width="100px;"/><br/><sub><b>DaiQiangReal</b></sub>](https://github.com/DaiQiangReal)<br/>|
|[<img src="https://avatars.githubusercontent.com/u/12951461?v=4" width="100px;"/><br/><sub><b>yisar</b></sub>](https://github.com/yisar)<br/>|[<img src="https://avatars.githubusercontent.com/u/60083015?v=4" width="100px;"/><br/><sub><b>hsp-sz</b></sub>](https://github.com/hsp-sz)<br/>|[<img src="https://avatars.githubusercontent.com/u/88357633?v=4" width="100px;"/><br/><sub><b>SunWuyuan</b></sub>](https://github.com/SunWuyuan)<br/>|[<img src="https://avatars.githubusercontent.com/u/46096697?v=4" width="100px;"/><br/><sub><b>uuiid</b></sub>](https://github.com/uuiid)<br/>|[<img src="https://avatars.githubusercontent.com/u/103258286?v=4" width="100px;"/><br/><sub><b>MengNianxiaoyao</b></sub>](https://github.com/MengNianxiaoyao)<br/>|[<img src="https://avatars.githubusercontent.com/u/37258062?v=4" width="100px;"/><br/><sub><b>zf1234d</b></sub>](https://github.com/zf1234d)<br/>|
[<img src="https://avatars.githubusercontent.com/u/157936029?v=4" width="100px;"/><br/><sub><b>ArcticFox520</b></sub>](https://github.com/ArcticFox520)<br/>|[<img src="https://avatars.githubusercontent.com/u/8605565?v=4" width="100px;"/><br/><sub><b>ysicing</b></sub>](https://github.com/ysicing)<br/>|[<img src="https://avatars.githubusercontent.com/u/2096890?v=4" width="100px;"/><br/><sub><b>cuiqg</b></sub>](https://github.com/cuiqg)<br/>|[<img src="https://avatars.githubusercontent.com/u/34783722?v=4" width="100px;"/><br/><sub><b>it-chenliang</b></sub>](https://github.com/it-chenliang)<br/>|[<img src="https://avatars.githubusercontent.com/u/1777211?v=4" width="100px;"/><br/><sub><b>wenerme</b></sub>](https://github.com/wenerme)<br/>

This project follows the git-contributor [spec](https://github.com/xudafeng/git-contributor), auto updated at `Sun Jun 02 2024 23:58:14 GMT+0800`.

<!-- GITCONTRIBUTOR_END -->
