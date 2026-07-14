# qa_python

'test_add_new_book_rejects_wrong_length_name' -  Валидация названия книги. Проверяется поведение при добавлении книг с длинными названиями и пустой строкой. Используется параметризация (@pytest.mark.parametrize) для нескольких значений.

test_add_new_book_rejects_duplicate_name' Проверяет, что добавить одну и ту же книгу дважды невозможно. В словаре books_genre остаётся только одна запись. 

test_set_book_genre_updates_genre_for_existing_book Проверяет, что для существующей книги устанавливается жанр. Словарь books_genre обновляется корректно. 

test_get_book_genre_get_right_genre Проверяет, что метод get_book_genre возвращает правильный жанр для конкретной книги. 

test_get_books_with_specific_genre_get_two_books проверяет возможность поиска книг по жанру. После добавления двух книг одного жанра метод возвращает список из двух названий. 

test_get_books_genre_return_dict_books_genre Проверяет, что метод возвращает полный словарь всех добавленных книг и их жанров. 

test_get_books_genre_returns_empty_dict_when_no_books При отсутствии книг метод возвращает пустой словарь 

test_get_books_for_children_add_books_for_children Проверяет, что книга с жанром «Мультфильмы» добавляется и корректно возвращается методом get_books_for_children

test_add_book_in_favorites_prevents_duplicate_in_favorites проверяет, что одну и ту же книгу нельзя добавить в избранное дважды. В списке она остаётся в единственном экземпляре. 

test_delete_book_from_favorites_book_is_removed_from_list Проверяет,что Книга удаляется из списка избранного. После вызова метода её нет в favorites

test_get_list_of_favorites_books_returns_empty_list_when_no_books Проверяет, что при отсутствии книг в избранном метод возвращает пустой список .