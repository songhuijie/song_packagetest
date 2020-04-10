## Packagetest-For-Laravel

[![license](https://img.shields.io/badge/license-WTFPL%20--%20Do%20What%20the%20Fuck%20You%20Want%20to%20Public%20License-green.svg)](https://raw.githubusercontent.com/ALawating-Rex/packagetest-for-laravel/master/LICENSE)

Just a test for laravel package development

用于 laravel 扩展包的开发学习

## Installation

```shell
$ composer require song/packagetest:dev-master
```


Publishing resources

```shell
php artisan vendor:publish --provider="Song\Packagetest\PackagetestServiceProvider"
```
Need to add in `config.app` 
`providers`
```shell
Illuminate\View\ViewServiceProvider::class
```
`aliases`
```shell
'Packagetest' => Song\Packagetest\Facades\Packagetest::class
```
**example of case**
```shell
return view('Packagetest::packagetest',['msg'=>Packagetest::test_rtn('Test')]);
```

## Documentation

## License

this repo is released under the [WTFPL](http://www.wtfpl.net/) – Do What the Fuck You Want to Public License.
