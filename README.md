import { createEvent, createStore } from 'effector'

const $count = createStore(0)

const increment = createEvent('increment')

$count.on(increment, (count) => count + 1)

$count.watch((count) => {
  console.log(`count is ${count}`)
}) // count is 0 (полезно для первичного рендера)

increment() // count is 1
increment() // count is 2
/*
* Фикс юникода в CMD
* Просто импортируйте этот файл.
* https://t.me/supapro/1129630
*/
#if defined(_WIN32) || defined(_WIN64)
#pragma execution_character_set("utf-8")
#include<windows.h>
const auto _dummy_ = []() {
    SetConsoleCP(65001);
    SetConsoleOutputCP(65001);
    return 0;
}();
#endif
/
////
.
